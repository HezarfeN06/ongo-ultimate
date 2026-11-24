# Mevcut kurulumu güncelleme

1. Uygulama dosyalarını, yüklemeleri ve veritabanını yedekleyin.
2. [Sürüm notlarını](../CHANGELOG.md) ve yayımdaki kurulum notlarını okuyun.
3. Güncel ZIP'in SHA-256 özetini doğrulayın.
4. Dosyaları mevcut web köküne aktarın. `config.php`, veritabanı, yüklemeler, çalışma zamanı lisans dosyaları ve `.user.ini` korunmalıdır.
5. Kurulu sitede `install.php` çalıştırmayın. Yönetici/müşteri girişlerini, kritik sayfaları ve lisans durumunu kontrol edin.

Başarısız güncellemede dosyaları ve veritabanını birlikte geri yükleyin.

`2026.11.23-r3` dağıtımında, önceki pakette eksik kalan `public-demo-admin.php` dosyası tamamlanmıştır. Genel hata ekranının sebebi destek koduyla incelenmelidir; tek başına PHP sürümü varsayımı yeterli değildir.
