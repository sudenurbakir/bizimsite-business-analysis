# BizimSite - Ortak Gider Yönetimi Use Case Analizi

BizimSite ortak gider yönetimi süreci kapsamında kullanıcılar ile sistem arasındaki temel etkileşimler aşağıda use case olarak tanımlanmıştır.

---

## UC-19 - Ortak Gider Kaydı Oluşturma

### Aktör

Muhasebe Sorumlusu

### Amaç

Siteye ait ortak gider bilgilerinin sistemde kayıt altına alınmasını sağlamak.

### Ön Koşullar

- Muhasebe sorumlusu sisteme giriş yapmış olmalıdır.
- Kullanıcının ortak gider kaydı oluşturma yetkisi bulunmalıdır.

### Tetikleyici

Muhasebe sorumlusunun yeni ortak gider kaydı oluşturmak istemesi.

### Ana Akış

1. Muhasebe sorumlusu ortak gider yönetimi ekranını açar.
2. Yeni ortak gider kaydı oluşturma işlemini başlatır.
3. Sistem ortak gider formunu görüntüler.
4. Muhasebe sorumlusu gider türü, dönem ve tutar bilgilerini girer.
5. Muhasebe sorumlusu kayıt işlemini başlatır.
6. Sistem girilen bilgileri doğrular.
7. Sistem ortak gider kaydını oluşturur.
8. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Zorunlu Alanların Eksik Olması

1. Sistem zorunlu alanların eksik olduğunu tespit eder.
2. Sistem ortak gider kaydını oluşturmaz.
3. Sistem kullanıcıya eksik alanlara ilişkin hata mesajı gösterir.

#### A2 - Bireysel Daire Giderinin Kaydedilmek İstenmesi

1. Sistem girilen gider bilgisinin bireysel daireye ait olduğunu tespit eder.
2. Sistem ortak gider kaydını oluşturmaz.
3. Sistem kullanıcıya ilgili giderin ortak gider olarak kaydedilemeyeceğini bildirir.

### Son Koşullar

- Ortak gider kaydı sistemde kayıt altına alınır.

### İlgili Kullanıcı Hikayesi

- US-20

---

## UC-20 - Ortak Gider Kaydını Güncelleme

### Aktör

Muhasebe Sorumlusu

### Amaç

Mevcut ortak gider bilgilerinin güncellenmesini sağlamak.

### Ön Koşullar

- Muhasebe sorumlusu sisteme giriş yapmış olmalıdır.
- İlgili ortak gider kaydı sistemde bulunmalıdır.
- Kullanıcının ortak gider kaydı güncelleme yetkisi bulunmalıdır.

### Tetikleyici

Muhasebe sorumlusunun mevcut bir ortak gider kaydını güncellemek istemesi.

### Ana Akış

1. Muhasebe sorumlusu ortak gider yönetimi ekranını açar.
2. Sistem ortak gider kayıtlarını görüntüler.
3. Muhasebe sorumlusu güncellenecek ortak gider kaydını seçer.
4. Sistem mevcut gider bilgilerini görüntüler.
5. Muhasebe sorumlusu gider bilgilerini düzenler.
6. Muhasebe sorumlusu güncelleme işlemini başlatır.
7. Sistem girilen bilgileri doğrular.
8. Sistem ortak gider kaydını günceller.
9. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Geçersiz veya Eksik Veri

1. Sistem girilen bilgilerin geçersiz veya eksik olduğunu tespit eder.
2. Sistem güncelleme işlemini gerçekleştirmez.
3. Sistem kullanıcıya hata mesajı gösterir.

### Son Koşullar

- Ortak gider kaydı güncel bilgiler ile sistemde saklanır.

### İlgili Kullanıcı Hikayesi

- US-21

---

## UC-21 - Ortak Gider Kaydını Yayımlama

### Aktör

Muhasebe Sorumlusu

### Amaç

Ortak gider kaydının site sakinlerinin erişimine sunulmasını sağlamak.

### Ön Koşullar

- Muhasebe sorumlusu sisteme giriş yapmış olmalıdır.
- İlgili ortak gider kaydı sistemde bulunmalıdır.
- Kullanıcının ortak gider kaydı yayımlama yetkisi bulunmalıdır.

### Tetikleyici

Muhasebe sorumlusunun bir ortak gider kaydını yayımlamak istemesi.

### Ana Akış

1. Muhasebe sorumlusu ortak gider yönetimi ekranını açar.
2. Yayımlanacak ortak gider kaydını seçer.
3. Sistem ortak gider bilgilerini görüntüler.
4. Muhasebe sorumlusu yayımlama işlemini başlatır.
5. Sistem kullanıcının yetkisini kontrol eder.
6. Sistem ortak gider kaydını yayımlar.
7. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Yetkisiz İşlem

1. Sistem kullanıcının ortak gider kaydı yayımlama yetkisine sahip olmadığını tespit eder.
2. Sistem yayımlama işlemini gerçekleştirmez.
3. Sistem erişim işlemini engeller.

### Son Koşullar

- Ortak gider kaydı yayımlanmış durumda sistemde saklanır.
- Ortak gider kaydı site sakinleri tarafından görüntülenebilir.

### İlgili Kullanıcı Hikayesi

- US-22

---

## UC-22 - Yayımlanmış Ortak Giderleri Görüntüleme

### Aktör

Site Sakini

### Amaç

Siteye ait yayımlanmış ortak gider bilgilerine erişilmesini sağlamak.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.

### Tetikleyici

Site sakininin ortak gider bilgilerini görüntülemek istemesi.

### Ana Akış

1. Site sakini ortak gider ekranını açar.
2. Sistem yayımlanmış ortak gider kayıtlarını getirir.
3. Sistem ortak gider kayıtlarını kullanıcıya görüntüler.
4. Site sakini görüntülemek istediği ortak gider kaydını seçer.
5. Sistem gider türü, dönem ve tutar bilgilerini görüntüler.

### Alternatif Akışlar

#### A1 - Yayımlanmış Ortak Gider Kaydı Bulunmaması

1. Sistem yayımlanmış ortak gider kaydı bulunmadığını tespit eder.
2. Sistem kullanıcıya görüntülenecek ortak gider kaydı bulunmadığını bildirir.

### Son Koşullar

- Site sakini yayımlanmış ortak gider bilgilerini görüntüler.

### İlgili Kullanıcı Hikayesi

- US-23

---

## Genel Değerlendirme

Ortak gider yönetimi use case analizi, muhasebe sorumlusunun siteye ait ortak gider kayıtlarını oluşturması, güncellemesi ve yayımlaması ile site sakinlerinin yayımlanmış ortak gider bilgilerine erişmesi süreçlerini açıklamaktadır.

Tanımlanan ana ve alternatif akışlar, sistem davranışlarının detaylandırılması ve sonraki tasarım çalışmalarında referans olarak kullanılacaktır.
