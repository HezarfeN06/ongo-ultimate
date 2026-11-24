# Sürüm notları

## 2026.11.23-r3

GitHub dağıtım yayını: **24 Kasım 2026**.

- Eksik `public-demo-admin.php` iki ürün paketine eklendi; demo yönetici girişindeki HTTP 500 düzeltildi.
- PHP sürümü ve temel uzantılar için çalışma öncesi gereksinim kontrolü eklendi.
- Tam dosya manifesti ve paket imza doğrulaması hazırlandı.
- Normal kurulum alanları sadeleştirildi: veritabanı, lisans ve yönetici e-posta/şifresi. Site adresi otomatik algılanır.

Kayıt portalında kalıcı kod gösterimi, 5 proje sınırı, alan adıyla doğrulama, sürüm yükleme ve sunucu izleme alanları bulunur. Portal ve lisans merkezi yönetim dosyaları bu herkese açık ürün paketine dahil değildir.

Kontroller: PHP 8.2.32 ve 8.4.23 üzerinde sözdizimi ve demo yönetim girişi; PHP 8.2 üzerinde ayrı veritabanlarında kurulum senaryoları. Gerçek ödeme, SMS gönderimi veya hosting açılışı dağıtım kontrolünde başlatılmadı.
