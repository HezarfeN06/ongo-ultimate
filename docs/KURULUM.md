# Kurulum rehberi

PHP 8.2+, MySQL/MariaDB ve HTTPS gerekir. PDO MySQL, cURL, OpenSSL, mbstring, DOM, fileinfo ve Session etkin olmalıdır. Kurulum alan adı dışarıdan HTTPS ile erişilebilir olmalıdır.

1. [Kayıt portalından](https://kayit.ongo.com.tr/lisans-olustur) hesabınızı ve alan adı lisansınızı oluşturun.
2. Tam kodunuzu **Lisans kodlarım** alanından kopyalayın.
3. [GitHub Releases](https://github.com/HezarfeN06/ongo-ultimate/releases/latest) veya [hesabınızın indirme alanından](https://kayit.ongo.com.tr/hesabim/indirmeler) `ongo-ultimate.zip` indirin.
4. Hosting panelinde boş veritabanı ve o veritabanına yetkili kullanıcı oluşturun.
5. ZIP içeriğini sitenin web köküne çıkarın; fazladan bir alt klasör oluşmadığını kontrol edin.
6. `https://alanadiniz.com/install.php` adresine girin. Veritabanı sunucusu, adı, kullanıcısı ve şifresini; lisans kodunu; yönetici e-postası ve şifresini girin.
7. Firma bilgileri, logo/favicon, ürünler, dönem fiyatları, menüler ve içerikleri yönetimden düzenleyin.

Site adresi otomatik algılanır. Yönetici şifresi en az 12 karakterdir. İlk lisans doğrulaması tamamlanmadan kurulum bitmez; kurulum sonrasında install.php kapanır.

Ters vekil kullanıyorsanız HTTPS bilgisini PHP'ye doğru aktarın. Sağlayıcıları kendi hesaplarınızla yapılandırın; gerçek ödeme ve hizmet işlemlerinden önce test ortamlarını kullanın.

## Zamanlanmış kontrol

Trafik almayan sitelerde günlük görev tanımlayın:

```sh
php /TAM/SITE/YOLU/cron/license-heartbeat.php
```

## Sık karşılaşılan durumlar

| Durum | Kontrol |
|---|---|
| Alan adı eşleşmiyor | Lisansın kayıtlı alan adı ve kurulum adresi |
| HTTPS doğrulanamıyor | Sertifika zinciri ve dış erişim; TLS doğrulamasını kapatmayın |
| Veritabanı bağlantısı reddediliyor | Kullanıcı yetkisi, sunucu adresi ve parola |
| Uzantı eksik | Hosting panelinde seçili PHP sürümünün uzantıları |
| Beklenmeyen hata | Destek koduyla özel destek talebi; yapılandırmanızı açık paylaşmayın |
