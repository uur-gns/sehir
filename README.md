# İsim Şehir

Kurulum gerektirmeyen, telefonlarda oynanabilen oda kodlu İsim Şehir oyunu.

## Oynama

1. Siteyi HTTPS destekleyen statik bir web sunucusunda yayınlayın.
2. Oyuncular siteyi kendi telefonlarında açsın.
3. Bir kişi adını yazıp **Oda oluştur** desin; çıkan 6 haneli kodu arkadaşlarıyla paylaşsın.
4. Diğerleri adını ve oda kodunu girip **Odaya katıl** desin.
5. Oda sahibi oyunu başlatsın. Cevaplar her oyuncunun kendi cihazında kalır; tur sonunda tüm oyuncular cevapları geçerli, aynı ya da geçersiz diye oylar.

Oyuncular ve oyun durumu tarayıcılar arasında WebRTC ile eşler arası taşınır. Bağlantı kurmak için PeerJS'in ücretsiz bulut sinyal sunucusu kullanılır. Oda sahibi sekmeyi açık tutmalıdır; bu prototip kapalı odalar için tasarlanmıştır ve kalıcı sunucu/veritabanı kullanmaz.

## Dosyalar

- `index.html` — arayüz ve stiller
- `online.js` — oda, eşler arası bağlantı ve oyun akışı

PeerJS istemcisi sayfada CDN'den yüklenir; yayın sırasında internet bağlantısı gerekir.
