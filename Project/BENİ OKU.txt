"Tenebris Stationary – Kırtasiye Yönetim ve Satış Sistemi"

Tenebris Stationary, kırtasiye mağazalarının tüm iş süreçlerini dijital ortamda yönetmek amacıyla geliştirilmiş, 
yetki tabanlı erişim mantığına sahip Windows Form tabanlı bir yönetim ve satış uygulamasıdır.
Uygulama, SQL Server ile entegre çalışır ve veri güvenliği için geliştiriciye özel MD5 + SHA512 hibrit şifreleme algoritması kullanır.
Arayüzdeki tüm bileşenler (button, textbox, combobox, picturebox, panel, togglebutton, radiobutton, searchTool, datetimepicker vb.) özel class yapıları ile tasarlanmıştır.
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
"Amaç"

Bu projenin temel amacı, tek bir kırtasiye mağazasındaki stok, satış, tedarikçi ve müşteri yönetimi işlemlerini kolaylaştırmak ve yetki bazlı iş bölümü sağlayarak verimliliği artırmaktır.
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
"Rol ve Arayüzler"

////
1. Mağaza Sahibi (Admin)
•	Kullanıcı ekleme, düzenleme ve silme.
•	Kullanıcı yetkilendirme (stok, fiyat belirleme, tedarikçi ekleme vb.).
•	İşlem geçmişi inceleme.
•	Personel ve müşterilere özel mesaj gönderme (yalnızca uygulama içinden görüntülenebilir).
•	Sistem genel ayarlarını yönetme.
•	Backup yönetim arayüzüne erişim (CTRL+TAB ile giriş, yalnızca kurucu admin veya uygulama şifresini bilen yetkililer).

////
2. Mağaza Çalışanı (Personel)
•	Yetkilere göre:
	o Stok giriş/çıkış.
	o Ürün satın alımı.
	o Tedarikçi, marka, model ekleme.
	o Fiyat güncelleme.
•	Admin tarafından gönderilen mesajları görüntüleme.

////
3. Mağaza Müşterisi (Müşteri)
•	Stokta bulunan ürünleri filtreleme ve sıralama.
•	Sepete ürün ekleme ve satın alma.
•	Kayıtlı kart ile tek tıkla ödeme veya manuel ödeme.
•	İade talebi oluşturma (iade sebebi belirtilerek).
•	Admin tarafından gönderilen mesajları görüntüleme.
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
"Uygulama Özel Yönetim Paneli"

Bu panel, yalnızca kurucu admin veya uygulama şifresini bilen yetkililer tarafından kullanılabilir.
Panel üzerinden yapılabilen işlemler:
•	Uygulama şifresi değiştirme.
•	Windows ile başlatma seçeneğini açma/kapatma.
•	Veritabanı yönetimi:
	o Sıfırlanmış veya seçilmiş veritabanı yükleme.
	o Veritabanı silme.
•	Lisans yönetimi:
	o Uygulama lisansları kullanıcıya bağlıdır.
	o Lisanslar tek cihaz kullanımına özel tasarlanmıştır.
	o Cihazların HWID bilgisi alınarak veritabanına kaydedilir.
	o HWID eşleşen cihazlarda lisans anahtarı istenmeden otomatik çalışır.
	o Kullanıcı farklı bir cihazdan giriş yapmak isterse lisans yeni cihaza bağlanır, eski cihazdaki HWID silinir ve yeni cihazın HWID’si kaydedilir.
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
"Teknik Özellikler"

•	Platform: Windows Forms (C#)
•	Veritabanı: Microsoft SQL Server
•	Şifreleme: MD5 + SHA512 hibrit, geliştiriciye özel algoritma.
•	Özel Bileşenler: Class tabanlı özelleştirilmiş button, textbox, combobox, picturebox, panel, togglebutton, radiobutton, searchTool, datetimepicker vb.
•	Güvenlik:
	o Yetki tabanlı erişim kontrolü.
	o HWID tabanlı lisanslama.
	o Şifreleme ile veri koruması.
•	Backup Yönetimi: Otomatik ve manuel yedekleme, panel üzerinden kontrol.
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
"Öne Çıkan Özellikler"

•	Çoklu rol desteği (Admin / Personel / Müşteri).
•	Gelişmiş stok, satın alma ve iade yönetimi.
•	Uygulama içi özel mesajlaşma sistemi.
•	HWID tabanlı güvenli lisanslama.
•	Özelleştirilmiş kullanıcı arayüzü.
•	Yönetim paneli ile detaylı sistem kontrolü.
