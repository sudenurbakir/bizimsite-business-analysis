# BizimSite - Ortak Gider Yönetimi Kullanıcı Hikayeleri

BizimSite ortak gider yönetimi süreci kapsamında kullanıcı ihtiyaçlarını sistem davranışlarına dönüştürmek amacıyla kullanıcı hikayeleri hazırlanmıştır.

Her kullanıcı hikayesi, ilgili kullanıcının hedefini ve bu hedef sonucunda elde etmek istediği değeri açıklamaktadır.

---

## US-19 - Ortak Gider Kaydı Oluşturma

### Kullanıcı Hikayesi

Bir muhasebe sorumlusu olarak, siteye ait ortak gider kaydı oluşturmak istiyorum; böylece ortak kullanım alanlarına ilişkin giderleri sistem üzerinden kayıt altına alabilirim.

### Kabul Kriterleri

- Muhasebe sorumlusu yeni ortak gider kaydı oluşturabilmelidir.
- Ortak gider kaydı gider türü, dönem ve tutar bilgisi içermelidir.
- Bireysel dairelere ait elektrik, su veya doğalgaz faturaları ortak gider olarak kaydedilememelidir.
- Zorunlu alanlar tamamlanmadan ortak gider kaydı oluşturulmamalıdır.
- Yetkisiz kullanıcılar ortak gider kaydı oluşturamamalıdır.
- Başarılı kayıt işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-05
- BRULE-19
- BRULE-20
- BRULE-21
- BRULE-22
- NFR-02
- NFR-11
- NFR-18

---

## US-20 - Ortak Gider Kaydını Güncelleme

### Kullanıcı Hikayesi

Bir muhasebe sorumlusu olarak, oluşturulan ortak gider kaydını güncellemek istiyorum; böylece gider bilgilerinde gerekli düzenlemeleri yapabilirim.

### Kabul Kriterleri

- Muhasebe sorumlusu ortak gider kayıtlarını güncelleyebilmelidir.
- Gider türü, dönem ve tutar bilgileri düzenlenebilmelidir.
- Geçersiz veya eksik veriler kaydedilmemelidir.
- Yetkisiz kullanıcılar ortak gider kayıtlarını güncelleyememelidir.
- Başarılı güncelleme işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-05
- BRULE-21
- BRULE-22
- NFR-02
- NFR-11
- NFR-19

---

## US-21 - Ortak Gider Kaydını Yayımlama

### Kullanıcı Hikayesi

Bir muhasebe sorumlusu olarak, oluşturulan ortak gider kaydını yayımlamak istiyorum; böylece site sakinlerinin ortak gider bilgilerine erişmesini sağlayabilirim.

### Kabul Kriterleri

- Muhasebe sorumlusu ortak gider kaydını yayımlayabilmelidir.
- Yayımlanan ortak gider kaydı site sakinleri tarafından görüntülenebilmelidir.
- Yayımlanmamış ortak gider kayıtları site sakinleri tarafından görüntülenememelidir.
- Yetkisiz kullanıcılar ortak gider kayıtlarını yayımlayamamalıdır.
- Başarılı yayımlama işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-05
- BRULE-23
- BRULE-24
- NFR-02
- NFR-11
- NFR-14

---

## US-22 - Yayımlanmış Ortak Giderleri Görüntüleme

### Kullanıcı Hikayesi

Bir site sakini olarak, yayımlanmış ortak gider kayıtlarını görüntülemek istiyorum; böylece siteye ait ortak giderler hakkında bilgi sahibi olabilirim.

### Kabul Kriterleri

- Site sakini yayımlanmış ortak gider kayıtlarını görüntüleyebilmelidir.
- Site sakini yayımlanmamış ortak gider kayıtlarını görüntüleyememelidir.
- Gider türü, dönem ve tutar bilgileri görüntülenebilmelidir.
- Ortak gider listesi tanımlanan kullanım koşulları altında en fazla 3 saniye içerisinde görüntülenmelidir.

### İlgili Gereksinimler

- BR-05
- BRULE-23
- BRULE-24
- NFR-05
- NFR-14

---

## Kullanıcı Hikayesi Özeti

| Kullanıcı Hikayesi | Rol | Amaç |
|---|---|---|
| US-19 | Muhasebe Sorumlusu | Ortak gider kaydı oluşturmak |
| US-20 | Muhasebe Sorumlusu | Ortak gider kaydını güncellemek |
| US-21 | Muhasebe Sorumlusu | Ortak gider kaydını yayımlamak |
| US-22 | Site Sakini | Yayımlanmış ortak giderleri görüntülemek |

---

## Genel Değerlendirme

Ortak gider yönetimi kullanıcı hikayeleri, muhasebe sorumlusunun siteye ait ortak gider kayıtlarını yönetmesi ve site sakinlerinin yayımlanmış ortak gider bilgilerine erişmesi temel alınarak hazırlanmıştır.

Tanımlanan kabul kriterleri, kullanıcı hikayelerinin tamamlanma koşullarının değerlendirilmesinde referans olarak kullanılacaktır.
