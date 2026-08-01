# Wen Gayrimenkul Sitesi — Kurulum Rehberi (Ferdi Alkan)

Bu pakette hazır bir web siteniz var. Aşağıdaki adımları takip ederek
**tek maliyet .com alan adı** olacak şekilde, ücretsiz yayına alabilirsiniz.

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

## 3. Adım — Yönetim panelini aktif edin

1. Netlify panelinde: **Site settings → Identity → Enable Identity**
2. Aynı sayfada **Services → Git Gateway → Enable Git Gateway**
3. `admin/config.yml` dosyasını GitHub üzerinden açıp şu satırı düzenleyin:
   ```
   repo: KULLANICI-ADINIZ/REPO-ADINIZ
   ```
   Kendi GitHub kullanıcı adınız ve deponun adıyla değiştirin, kaydedin.
4. Artık `siteniz.com/admin/` (veya `rastgele-isim.netlify.app/admin/`)
   adresinden giriş yapıp:
   - Site Ayarları → telefon, e-posta, adres, ana başlık
   - İlanlar → ilan ekleme/silme/düzenleme
   yapabilirsiniz. Kaydettiğinizde site birkaç saniye içinde otomatik güncellenir.

## 4. Adım — .com alan adınızı bağlayın

1. Aldığınız .com alan adını satın aldığınız yerden (Turhost, Natro, GoDaddy vb.) yönetin.
2. Netlify panelinde **Domain settings → Add a domain** deyip alan adınızı yazın.
3. Netlify size 2 tane "DNS kaydı" (nameserver veya A/CNAME) verecek —
   bunları alan adını aldığınız firmanın panelindeki DNS ayarlarına eklersiniz.
   (Bu adımda firma ile görüştüğünüzde "Netlify'a yönlendirme yapacağım" demeniz yeterli,
   çoğu firma bunu telefonla da yapıyor.)
4. Bağlantı birkaç saat içinde aktif olur — siteniz artık kendi alan adınızda yayında.

---

## Form yanıtlarını görme

Sitenizdeki "Bilgi Formu"nu dolduran kişiler otomatik olarak Netlify hesabınıza düşer.
Görmek için: Netlify panelinde sitenizi açın → üst menüden **"Forms"** sekmesine tıklayın →
**"lead-form"** listesinde kimin ne zaman, hangi bilgilerle form gönderdiğini görürsünüz.
(Bu, Yönetim panelinden ayrı, Netlify hesabınızın kendi ekranıdır — ekstra kuruluma gerek yok.)

## Toplam maliyet
- .com alan adı: yıllık ~150-400 TL (tek ödemeniz)
- GitHub: ücretsiz
- Netlify barındırma: ücretsiz
- Yönetim paneli: ücretsiz

## Yardım gerekirse
Bu adımlardan herhangi birinde takılırsanız, ekran görüntüsü paylaşıp
buradan devam edebiliriz — birlikte tamamlarız.
