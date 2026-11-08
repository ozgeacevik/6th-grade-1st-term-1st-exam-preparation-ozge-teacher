# Özge Teacher — Sınava Hazırlık Atölyesi

Mobil uyumlu, 6. sınıf İngilizce sınav hazırlık uygulaması. Uygulama GitHub Pages ile yayımlanabilir ve ziyaret edildikten sonra çevrimdışı da açılabilmesi için temel dosyaları önbelleğe alır.

## GitHub Pages'e yayımlama

1. GitHub'da yeni bir repository oluşturun (ör. `ozge-teacher-english`). Ücretsiz ve en kolay Pages kurulumu için repository'yi **Public** seçin.
2. Bu klasördeki `index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg` ve `.nojekyll` dosyalarını repository'nin en üst dizinine yükleyin. `README.md` de eklenebilir.
3. Repository'de **Settings → Pages** bölümünü açın.
4. **Build and deployment** altında **Deploy from a branch** seçin; branch olarak `main`, klasör olarak `/(root)` seçip **Save**'e basın.
5. GitHub Pages adresi birkaç dakika içinde hazır olur: `https://GITHUB-KULLANICI-ADINIZ.github.io/REPOSITORY-ADI/`.
6. Bu bağlantıyı telefonunuzda açın. İsterseniz tarayıcının menüsünden **Ana ekrana ekle / Install app** seçeneğiyle uygulama gibi kullanın.

Her yeni sürümde dosyaları aynı repository'ye yükleyip commit edin; Pages otomatik olarak yeniden yayımlar.

## Çevrimdışı kullanım ve ilerleme

Uygulama ziyaret edildikten sonra service worker temel uygulama dosyalarını önbelleğe alır; internet bağlantısı kesilirse daha önce yüklenen sürüm açılabilir. Quiz puanları ve ilerleme `localStorage` ile **yalnızca kullanılan tarayıcı/cihazda** saklanır. Bu sürümde hesap, sunucu tabanlı veri kaydı veya cihazlar arası eşitleme bulunmaz. Telefonla bilgisayar arasında ilerleme paylaşımı için ayrıca güvenli bir backend/veri eşitleme özelliği geliştirmek gerekir.

## Dosyalar

- `index.html` — uygulama ve içerik
- `manifest.webmanifest` — ana ekrana ekleme/PWA bilgileri
- `sw.js` — çevrimdışı önbellek
- `icon.svg` — uygulama simgesi
- `.nojekyll` — GitHub Pages'in dosyaları doğrudan yayımlaması için
