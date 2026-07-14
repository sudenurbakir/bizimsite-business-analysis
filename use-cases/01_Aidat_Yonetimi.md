# BizimSite - Aidat Yönetimi Use Case Analizi

BizimSite aidat yönetimi süreci kapsamında kullanıcılar ile sistem arasındaki temel etkileşimler aşağıda use case olarak tanımlanmıştır.

---

## UC-01 - Aidat Kaydı Oluşturma

### Aktör

Muhasebe Sorumlusu

### Amaç

Bir daireye ait aidat kaydının sistemde oluşturulmasını sağlamak.

### Ön Koşullar

- Muhasebe sorumlusu sisteme giriş yapmış olmalıdır.
- Kullanıcının aidat kaydı oluşturma yetkisi bulunmalıdır.
- İlgili daire sistemde kayıtlı olmalıdır.

### Tetikleyici

Muhasebe sorumlusunun yeni aidat kaydı oluşturma işlemini başlatması.

### Ana Akış

1. Muhasebe sorumlusu aidat yönetimi ekranını görüntüler.
2. Yeni aidat kaydı oluşturma işlemini başlatır.
3. Sistem aidat kayıt formunu görüntüler.
4. Muhasebe sorumlusu ilgili daireyi seçer.
5. Aidat dönemi ve gerekli aidat bilgilerini girer.
6. Muhasebe sorumlusu kayıt işlemini başlatır.
7. Sistem girilen bilgileri doğrular.
8. Sistem aidat kaydını oluşturur.
9. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Zorunlu Alanların Eksik Olması

1. Sistem zorunlu alanların eksik olduğunu tespit eder.
2. Sistem aidat kaydını oluşturmaz.
3. Sistem kullanıcıya eksik alanlara ilişkin hata mesajı gösterir.

#### A2 - Geçersiz Veri Girilmesi

1. Sistem girilen verilerin geçersiz olduğunu tespit eder.
2. Sistem aidat kaydını oluşturmaz.
3. Sistem kullanıcıya anlaşılır bir hata mesajı gösterir.

### Son Koşullar

- Aidat kaydı ilgili daire ve aidat dönemi ile ilişkilendirilmiş şekilde sistemde kayıt altına alınır.

### İlgili Kullanıcı Hikayesi

- US-01

---

## UC-02 - Aidat Ödeme Durumunu Güncelleme

### Aktör

Muhasebe Sorumlusu

### Amaç

Bir aidat kaydının güncel ödeme durumunun sistemde takip edilmesini sağlamak.

### Ön Koşullar

- Muhasebe sorumlusu sisteme giriş yapmış olmalıdır.
- İlgili aidat kaydı sistemde bulunmalıdır.
- Kullanıcının aidat kaydını güncelleme yetkisi bulunmalıdır.

### Tetikleyici

Muhasebe sorumlusunun bir aidat kaydının ödeme durumunu güncellemek istemesi.

### Ana Akış

1. Muhasebe sorumlusu aidat kayıtlarını görüntüler.
2. Güncellenecek aidat kaydını seçer.
3. Sistem aidat kaydının mevcut bilgilerini görüntüler.
4. Muhasebe sorumlusu ödeme durumunu günceller.
5. Muhasebe sorumlusu güncelleme işlemini başlatır.
6. Sistem yeni ödeme durumunu doğrular.
7. Sistem aidat kaydını günceller.
8. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Geçersiz Ödeme Durumu

1. Sistem ödeme durumunun tanımlı değerlerden biri olmadığını tespit eder.
2. Sistem güncelleme işlemini gerçekleştirmez.
3. Sistem kullanıcıya hata mesajı gösterir.

### Son Koşullar

- Aidat kaydının ödeme durumu güncel bilgi ile sistemde saklanır.

### İlgili Kullanıcı Hikayesi

- US-02

---

## UC-03 - Kendi Aidat Bilgilerini Görüntüleme

### Aktör

Site Sakini

### Amaç

Site sakininin kendi dairesine ait aidat ve ödeme bilgilerini görüntülemesini sağlamak.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.
- Site sakini bir daire ile ilişkilendirilmiş olmalıdır.

### Tetikleyici

Site sakininin aidat bilgilerini görüntülemek istemesi.

### Ana Akış

1. Site sakini aidat bilgileri ekranını açar.
2. Sistem kullanıcının ilişkili olduğu daireyi belirler.
3. Sistem ilgili daireye ait aidat kayıtlarını getirir.
4. Sistem aidat dönemi ve ödeme durumu bilgilerini görüntüler.

### Alternatif Akışlar

#### A1 - Aidat Kaydı Bulunmaması

1. Sistem ilgili daireye ait aidat kaydı bulunmadığını tespit eder.
2. Sistem kullanıcıya görüntülenecek aidat kaydı bulunmadığını bildirir.

### Son Koşullar

- Site sakini kendi dairesine ait mevcut aidat bilgilerini görüntüler.

### İlgili Kullanıcı Hikayesi

- US-03

---

## UC-04 - Aidat Kayıtlarını Görüntüleme

### Aktörler

- Site Yöneticisi
- Muhasebe Sorumlusu

### Amaç

Yetkili kullanıcıların siteye ait aidat kayıtlarını görüntülemesini ve takip etmesini sağlamak.

### Ön Koşullar

- Kullanıcı sisteme giriş yapmış olmalıdır.
- Kullanıcının aidat kayıtlarını görüntüleme yetkisi bulunmalıdır.

### Tetikleyici

Yetkili kullanıcının aidat kayıtlarını görüntülemek istemesi.

### Ana Akış

1. Kullanıcı aidat yönetimi ekranını açar.
2. Sistem kullanıcının erişim yetkisini kontrol eder.
3. Sistem aidat kayıtlarını getirir.
4. Sistem aidat kayıtlarını kullanıcıya görüntüler.

### Alternatif Akışlar

#### A1 - Yetkisiz Erişim

1. Sistem kullanıcının gerekli erişim yetkisine sahip olmadığını tespit eder.
2. Sistem aidat kayıtlarını görüntülemez.
3. Sistem erişim işlemini engeller.

#### A2 - Aidat Kaydı Bulunmaması

1. Sistem görüntülenecek aidat kaydı bulunmadığını tespit eder.
2. Sistem kullanıcıya kayıt bulunmadığını bildirir.

### Son Koşullar

- Yetkili kullanıcı mevcut aidat kayıtlarını görüntüler.

### İlgili Kullanıcı Hikayesi

- US-04

---

## Genel Değerlendirme

Aidat yönetimi use case analizi, muhasebe sorumlusunun aidat kayıtlarını oluşturması ve güncellemesi ile site sakinleri ve yetkili kullanıcıların aidat bilgilerine erişim süreçlerini açıklamaktadır.

Tanımlanan ana ve alternatif akışlar, sistem davranışlarının detaylandırılması ve sonraki tasarım çalışmalarında referans olarak kullanılacaktır.
