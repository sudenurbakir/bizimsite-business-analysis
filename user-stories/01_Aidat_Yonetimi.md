# BizimSite - Aidat Yönetimi Kullanıcı Hikâyeleri

BizimSite aidat yönetimi süreci kapsamında kullanıcı ihtiyaçlarını sistem davranışlarına dönüştürmek amacıyla kullanıcı hikâyeleri hazırlanmıştır.

Her kullanıcı hikayesi, ilgili kullanıcının hedefini ve bu hedef sonucunda elde etmek istediği değeri açıklamaktadır.

---

## US-01 - Aidat Kaydı Oluşturma

### Kullanıcı Hikayesi

Bir muhasebe sorumlusu olarak, yeni aidat kaydı oluşturmak istiyorum; böylece dairelere ait aidat bilgilerini sistem üzerinden takip edebilirim.

### Kabul Kriterleri

- Muhasebe sorumlusu yeni aidat kaydı oluşturabilmelidir.
- Aidat kaydı bir daire ile ilişkilendirilmelidir.
- Aidat kaydı bir aidat dönemi ile ilişkilendirilmelidir.
- Zorunlu alanlar tamamlanmadan aidat kaydı oluşturulmamalıdır.
- Başarılı kayıt işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-01
- FR-01
- FR-02
- NFR-11
- NFR-18

---

## US-02 - Aidat Ödeme Durumunu Güncelleme

### Kullanıcı Hikayesi

Bir muhasebe sorumlusu olarak, aidat kaydının ödeme durumunu güncellemek istiyorum; böylece güncel ödeme bilgilerini sistem üzerinden takip edebilirim.

### Kabul Kriterleri

- Muhasebe sorumlusu aidat ödeme durumunu güncelleyebilmelidir.
- Güncellenen ödeme durumu ilgili aidat kaydı ile ilişkilendirilmelidir.
- Başarılı güncelleme işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.
- Yetkisiz kullanıcılar aidat ödeme durumunu güncelleyememelidir.

### İlgili Gereksinimler

- BR-01
- FR-03
- FR-40
- NFR-02
- NFR-11

---

## US-03 - Kendi Aidat Bilgilerini Görüntüleme

### Kullanıcı Hikayesi

Bir site sakini olarak, kendi daireme ait aidat bilgilerini görüntülemek istiyorum; böylece site yönetimine ulaşmadan aidat ve ödeme durumumu kontrol edebilirim.

### Kabul Kriterleri

- Site sakini kendi dairesine ait aidat kayıtlarını görüntüleyebilmelidir.
- Aidat dönemi görüntülenebilmelidir.
- Aidat ödeme durumu görüntülenebilmelidir.
- Site sakini başka bir daireye ait aidat bilgilerini görüntüleyememelidir.
- Aidat bilgileri tanımlanan kullanım koşulları altında en fazla 3 saniye içerisinde görüntülenmelidir.

### İlgili Gereksinimler

- BR-01
- FR-04
- FR-41
- NFR-05
- NFR-12
- NFR-13

---

## US-04 - Aidat Kayıtlarını Görüntüleme

### Kullanıcı Hikayesi

Bir site yöneticisi veya muhasebe sorumlusu olarak, aidat kayıtlarını görüntülemek istiyorum; böylece siteye ait aidat süreçlerini takip edebilirim.

### Kabul Kriterleri

- Site yöneticisi aidat kayıtlarını görüntüleyebilmelidir.
- Muhasebe sorumlusu aidat kayıtlarını görüntüleyebilmelidir.
- Yetkisiz kullanıcılar yönetim kapsamındaki aidat kayıtlarına erişememelidir.
- Aidat kayıtları tanımlanan kullanım koşulları altında en fazla 3 saniye içerisinde görüntülenmelidir.

### İlgili Gereksinimler

- BR-01
- FR-05
- FR-40
- NFR-05
- NFR-12
- NFR-13

---

## Kullanıcı Hikayesi Özeti

| Kullanıcı Hikâyesi | Rol | Amaç |
|---|---|---|
| US-01 | Muhasebe Sorumlusu | Aidat kaydı oluşturmak |
| US-02 | Muhasebe Sorumlusu | Ödeme durumunu güncellemek |
| US-03 | Site Sakini | Kendi aidat bilgilerini görüntülemek |
| US-04 | Site Yöneticisi / Muhasebe Sorumlusu | Aidat kayıtlarını takip etmek |

---

## Genel Değerlendirme

Aidat yönetimi kullanıcı hikayeleri, muhasebe sorumlusunun aidat kayıtlarını yönetmesi ve site sakinlerinin kendi dairelerine ait aidat bilgilerine erişebilmesi temel alınarak hazırlanmıştır.

Tanımlanan kabul kriterleri, kullanıcı hikâyelerinin tamamlanma koşullarının değerlendirilmesinde referans olarak kullanılacaktır.
