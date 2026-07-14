# BizimSite - Duyuru Yönetimi Use Case Analizi

BizimSite duyuru yönetimi süreci kapsamında kullanıcılar ile sistem arasındaki temel etkileşimler aşağıda use case olarak tanımlanmıştır.

---

## UC-05 - Duyuru Oluşturma

### Aktör

Site Yöneticisi

### Amaç

Site sakinlerine iletilecek bir duyurunun sistemde oluşturulmasını sağlamak.

### Ön Koşullar

- Site yöneticisi sisteme giriş yapmış olmalıdır.
- Kullanıcının duyuru oluşturma yetkisi bulunmalıdır.

### Tetikleyici

Site yöneticisinin yeni duyuru oluşturma işlemini başlatması.

### Ana Akış

1. Site yöneticisi duyuru yönetimi ekranını açar.
2. Yeni duyuru oluşturma işlemini başlatır.
3. Sistem duyuru formunu görüntüler.
4. Site yöneticisi başlık ve içerik bilgilerini girer.
5. Site yöneticisi kayıt işlemini başlatır.
6. Sistem girilen bilgileri doğrular.
7. Sistem duyuruyu kaydeder.
8. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Zorunlu Alanların Eksik Olması

1. Sistem zorunlu alanların eksik olduğunu tespit eder.
2. Sistem duyuruyu kaydetmez.
3. Sistem kullanıcıya eksik alanlara ilişkin hata mesajı gösterir.

### Son Koşullar

- Duyuru sistemde kayıt altına alınır.

### İlgili Kullanıcı Hikayesi

- US-05

---

## UC-06 - Taslak Duyuruyu Görüntüleme ve Düzenleme

### Aktör

Site Yöneticisi

### Amaç

Taslak durumundaki bir duyurunun yayımlanmadan önce görüntülenmesini ve düzenlenmesini sağlamak.

### Ön Koşullar

- Site yöneticisi sisteme giriş yapmış olmalıdır.
- İlgili taslak duyuru sistemde bulunmalıdır.
- Kullanıcının duyuru yönetimi yetkisi bulunmalıdır.

### Tetikleyici

Site yöneticisinin bir taslak duyuruyu düzenlemek istemesi.

### Ana Akış

1. Site yöneticisi duyuru yönetimi ekranını açar.
2. Sistem taslak duyuruları görüntüler.
3. Site yöneticisi düzenlemek istediği taslak duyuruyu seçer.
4. Sistem duyurunun mevcut bilgilerini görüntüler.
5. Site yöneticisi başlık veya içerik bilgisini düzenler.
6. Site yöneticisi güncelleme işlemini başlatır.
7. Sistem girilen bilgileri doğrular.
8. Sistem taslak duyuruyu günceller.
9. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Geçersiz veya Eksik Veri

1. Sistem girilen bilgilerin geçersiz veya eksik olduğunu tespit eder.
2. Sistem güncelleme işlemini gerçekleştirmez.
3. Sistem kullanıcıya hata mesajı gösterir.

### Son Koşullar

- Taslak duyuru güncel bilgiler ile sistemde saklanır.
- Duyuru site sakinleri tarafından görüntülenemez.

### İlgili Kullanıcı Hikayesi

- US-06

---

## UC-07 - Duyuru Yayımlama

### Aktör

Site Yöneticisi

### Amaç

Hazırlanan bir duyurunun site sakinlerinin erişimine sunulmasını sağlamak.

### Ön Koşullar

- Site yöneticisi sisteme giriş yapmış olmalıdır.
- İlgili duyuru sistemde bulunmalıdır.
- Kullanıcının duyuru yayımlama yetkisi bulunmalıdır.

### Tetikleyici

Site yöneticisinin bir duyuruyu yayımlamak istemesi.

### Ana Akış

1. Site yöneticisi duyuru yönetimi ekranını açar.
2. Yayımlanacak duyuruyu seçer.
3. Sistem duyuru bilgilerini görüntüler.
4. Site yöneticisi yayımlama işlemini başlatır.
5. Sistem kullanıcının yetkisini kontrol eder.
6. Sistem duyuruyu yayımlar.
7. Sistem yayımlanma tarihini kayıt altına alır.
8. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Yetkisiz İşlem

1. Sistem kullanıcının duyuru yayımlama yetkisine sahip olmadığını tespit eder.
2. Sistem yayımlama işlemini gerçekleştirmez.
3. Sistem erişim işlemini engeller.

### Son Koşullar

- Duyuru yayımlanmış durumda sistemde saklanır.
- Duyuru site sakinleri tarafından görüntülenebilir.

### İlgili Kullanıcı Hikayesi

- US-07

---

## UC-08 - Yayımlanmış Duyuruları Görüntüleme

### Aktör

Site Sakini

### Amaç

Site yönetimi tarafından yayımlanan duyurulara erişilmesini sağlamak.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.

### Tetikleyici

Site sakininin duyuruları görüntülemek istemesi.

### Ana Akış

1. Site sakini duyuru ekranını açar.
2. Sistem yayımlanmış duyuruları getirir.
3. Sistem duyuruları kullanıcıya görüntüler.
4. Site sakini görüntülemek istediği duyuruyu seçer.
5. Sistem duyurunun başlık, içerik ve yayımlanma tarihi bilgilerini görüntüler.

### Alternatif Akışlar

#### A1 - Yayımlanmış Duyuru Bulunmaması

1. Sistem yayımlanmış duyuru bulunmadığını tespit eder.
2. Sistem kullanıcıya görüntülenecek duyuru bulunmadığını bildirir.

### Son Koşullar

- Site sakini yayımlanmış duyuru bilgilerini görüntüler.

### İlgili Kullanıcı Hikayesi

- US-08

---

## Genel Değerlendirme

Duyuru yönetimi use case analizi, site yöneticisinin duyuru oluşturma, taslak duyuruları düzenleme ve duyuru yayımlama süreçleri ile site sakinlerinin yayımlanmış duyurulara erişim sürecini açıklamaktadır.

Tanımlanan ana ve alternatif akışlar, sistem davranışlarının detaylandırılması ve sonraki tasarım çalışmalarında referans olarak kullanılacaktır.
