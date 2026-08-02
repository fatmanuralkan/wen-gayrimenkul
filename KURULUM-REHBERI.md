# Wen Gayrimenkul Sitesi — Kurulum Rehberi (Ferdi Alkan)

Bu pakette hazır bir web siteniz var. Aşağıdaki adımları takip ederek
**tek maliyet .com.tr alan adı** olacak şekilde, ücretsiz yayına alabilirsiniz.

Dosyalar:
- `index.html` → ana sayfa
- `assets/ferdi-alkan.jpg` → fotoğrafınız
- `data/settings.json` → telefon, e-posta, adres, ana başlık gibi bilgiler
- `data/listings.json` → ilanlarınız
- `admin/` → Yönetim paneli (Decap CMS)

---

## 1. Adım — GitHub hesabı açın (ücretsiz)

1. github.com adresine gidin, ücretsiz bir hesap açın.
2. Yeni bir **repository (depo)** oluşturun, adını örneğin `wen-gayrimenkul` koyun.
3. Bu klasördeki tüm dosyaları o depoya yükleyin (GitHub'ın "Add file → Upload files"
   seçeneğiyle sürükle-bırak yapabilirsiniz — kod bilmenize gerek yok).

## 2. Adım — Netlify'a bağlayın (ücretsiz barındırma)

1. netlify.com adresine gidin, "Sign up" ile GitHub hesabınızla giriş yapın.
2. "Add new site → Import an existing project" deyin, biraz önce oluşturduğunuz
   GitHub deposunu seçin.
3. Ayar sormadan "Deploy" butonuna basın — birkaç saniyede siteniz
   `rastgele-isim.netlify.app` gibi bir adreste yayında olacak.

## 3. Adım — Yönetim panelini aktif edin (kullanıcı adı/şifre ile giriş)

1. Netlify panelinde: **Site configuration → Identity → Enable Identity**
2. Aynı sayfada **Identity → Services → Git Gateway → Enable Git Gateway**
3. Yine Identity ayarlarında **"Registration"** kısmını **"Invite only"** yapın
   (böylece sadece sizin davet ettiğiniz kişi giriş yapabilir, başkası kayıt olamaz).
4. **Identity → Invite users** deyip kendi e-posta adresinizi
   (`ferdi.alkan@hotmail.com.tr`) girip davet gönderin.
5. E-postanıza gelen daveti açın, linke tıklayın — sizi siteye götürecek ve
   bir **şifre belirlemenizi** isteyecek.
6. Şifreyi belirledikten sonra artık `siteniz.com.tr/admin/` adresine gidip
   **e-posta + şifrenizle** giriş yapabilirsiniz — GitHub hesabına gerek kalmadan.
7. Giriş yaptığınızda:
   - **Site Ayarları** → telefon, e-posta, adres, ana başlık, hakkımda metni
   - **İlanlar** → ilan ekleme/silme/düzenleme
   - **Galeri** → fotoğraf ekleme/silme
   düzenleyebilirsiniz. Kaydettiğinizde site birkaç saniye içinde otomatik güncellenir.

## 4. Adım — arsacibaskan.com.tr alan adınızı bağlayın

`.com.tr` uzantısı `.com`'dan farklı olarak Türkiye'de faaliyet gösteren
kayıt firmaları üzerinden alınır ve genelde TC kimlik numarası istenir
(şirketiniz varsa vergi numarası da kullanılabilir).

1. Turhost, Natro, isimtescil.com.tr gibi bir firmadan **arsacibaskan.com.tr**
   alan adını satın alın.
2. Netlify panelinde **Domain management → Add a domain** deyip
   `arsacibaskan.com.tr` yazın.
3. Netlify size **nameserver** (isim sunucusu) bilgileri verecek.
4. Alan adını aldığınız firmanın panelinden (veya firmayı arayıp) bu
   nameserver'ları girmelerini isteyin — "Netlify'a yönlendirme yapacağım" demeniz yeterli.
5. Bağlantı birkaç saat (bazen 24 saate kadar) içinde aktif olur —
   siteniz artık **arsacibaskan.com.tr** adresinde yayında olur.

---

## Form yanıtlarını görme

Sitenizde 2 form var:
- **"lead-form"** → Bilgi Formu (mülk arayan müşteriler)
- **"degerlendirme-form"** → Mülk Değerlendirme Talebi (mülkünü satmak isteyenler)

Bu formları dolduran kişiler otomatik olarak Netlify hesabınıza düşer.
Görmek için: Netlify panelinde sitenizi açın → sol menüden **"Forms"** sekmesine tıklayın →
her iki formu da ayrı ayrı listede görürsünüz.
(Bu, Yönetim panelinden ayrı, Netlify hesabınızın kendi ekranıdır — ekstra kuruluma gerek yok.)

## Toplam maliyet
- .com.tr alan adı: yıllık ~200-500 TL (tek ödemeniz)
- GitHub: ücretsiz
- Netlify barındırma: ücretsiz
- Yönetim paneli (Netlify Identity): ücretsiz (ayda 5 kullanıcıya kadar)

## Yardım gerekirse
Bu adımlardan herhangi birinde takılırsanız, ekran görüntüsü paylaşıp
buradan devam edebiliriz — birlikte tamamlarız.
