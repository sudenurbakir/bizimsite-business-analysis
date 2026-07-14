# BizimSite - Duyuru Yönetimi Kullanıcı Hikayeleri

BizimSite duyuru yönetimi süreci kapsamında kullanıcı ihtiyaçlarını sistem davranışlarına dönüştürmek amacıyla kullanıcı hikayeleri hazırlanmıştır.

Her kullanıcı hikayesi, ilgili kullanıcının hedefini ve bu hedef sonucunda elde etmek istediği değeri açıklamaktadır.

---

## US-05 - Duyuru Oluşturma

### Kullanıcı Hikayesi

Bir site yöneticisi olarak, yeni bir duyuru oluşturmak istiyorum; böylece site sakinlerine iletilmesi gereken bilgileri sistem üzerinden hazırlayabilirim.

### Kabul Kriterleri

- Site yöneticisi yeni duyuru oluşturabilmelidir.
- Duyuru başlık ve içerik bilgilerini içermelidir.
- Zorunlu alanlar tamamlanmadan duyuru oluşturulmamalıdır.
- Yetkisiz kullanıcılar duyuru oluşturamamalıdır.
- Başarılı kayıt işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-02
- FR-06
- FR-44
- NFR-02
- NFR-11
- NFR-18

---

## US-06 - Duyuruyu Taslak Olarak Kaydetme ve Düzenleme

### Kullanıcı Hikayesi

Bir site yöneticisi olarak, hazırladığım duyuruyu taslak olarak kaydetmek ve daha sonra düzenlemek istiyorum; böylece duyuruyu yayımlamadan önce içerik üzerinde çalışmaya devam edebilirim.

### Kabul Kriterleri

- Site yöneticisi oluşturduğu duyuruyu taslak olarak kaydedebilmelidir.
- Taslak duyuru site sakinleri tarafından görüntülenememelidir.
- Site yöneticisi taslak duyuruyu daha sonra görüntüleyebilmelidir.
- Site yöneticisi taslak duyurunun başlık ve içerik bilgilerini düzenleyebilmelidir.
- Başarılı güncelleme işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-02
- FR-07
- FR-08
- FR-10
- NFR-02
- NFR-11
---

## US-07 - Duyuru Yayımlama

### Kullanıcı Hikayesi

Bir site yöneticisi olarak, hazırladığım duyuruyu yayımlamak istiyorum; böylece site sakinlerinin güncel duyuruya erişmesini sağlayabilirim.

### Kabul Kriterleri

- Site yöneticisi bir duyuruyu yayımlayabilmelidir.
- Yayımlanan duyurunun yayımlanma tarihi kayıt altına alınmalıdır.
- Yayımlanan duyuru site sakinleri tarafından görüntülenebilmelidir.
- Yetkisiz kullanıcılar duyuru yayımlayamamalıdır.
- Başarılı yayımlama işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-02
- FR-09
- FR-10
- FR-11
- FR-44
- NFR-02
- NFR-11

---

## US-08 - Yayımlanmış Duyuruları Görüntüleme

### Kullanıcı Hikayesi

Bir site sakini olarak, yayımlanmış duyuruları görüntülemek istiyorum; böylece site yönetimi tarafından paylaşılan güncel bilgilere erişebilirim.

### Kabul Kriterleri

- Site sakini yayımlanmış duyuruları görüntüleyebilmelidir.
- Site sakini taslak duyuruları görüntüleyememelidir.
- Duyurunun başlığı, içeriği ve yayımlanma tarihi görüntülenebilmelidir.
- Geçmiş yayımlanmış duyurular görüntülenebilmelidir.
- Duyuru listesi tanımlanan kullanım koşulları altında en fazla 3 saniye içerisinde görüntülenmelidir.

### İlgili Gereksinimler

- BR-02
- FR-10
- FR-11
- FR-12
- NFR-05

---

## Kullanıcı Hikayesi Özeti

| Kullanıcı Hikayesi | Rol | Amaç |
|---|---|---|
| US-05 | Site Yöneticisi | Duyuru oluşturmak |
| US-06 | Site Yöneticisi | Duyuruyu taslak olarak kaydetmek ve düzenlemek|
| US-07 | Site Yöneticisi | Duyuru yayımlamak |
| US-08 | Site Sakini | Yayımlanmış duyuruları görüntülemek |

---

## Genel Değerlendirme

Duyuru yönetimi kullanıcı hikayeleri, site yöneticisinin duyuru hazırlama ve yayımlama süreçleri ile site sakinlerinin yayımlanmış duyurulara erişim ihtiyaçları temel alınarak hazırlanmıştır.

Tanımlanan kabul kriterleri, kullanıcı hikayelerinin tamamlanma koşullarının değerlendirilmesinde referans olarak kullanılacaktır.
