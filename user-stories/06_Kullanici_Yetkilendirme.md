# BizimSite - Kullanıcı Yetkilendirme Kullanıcı Hikayeleri

BizimSite kullanıcı yetkilendirme süreci kapsamında kullanıcıların sistem içerisindeki işlem ve veri erişimlerinin sahip oldukları roller doğrultusunda sınırlandırılmasına yönelik kullanıcı hikayeleri hazırlanmıştır.

Her kullanıcı hikayesi, ilgili kullanıcının hedefini ve bu hedef sonucunda elde etmek istediği değeri açıklamaktadır.

---

## US-23 - Rol Kapsamındaki İşlemlere Erişim

### Kullanıcı Hikayesi

Bir sistem kullanıcısı olarak, sahip olduğum rol kapsamında izin verilen işlemlere erişmek istiyorum; böylece sistemde yalnızca yetkili olduğum işlemleri gerçekleştirebilirim.

### Kabul Kriterleri

- Kullanıcı yalnızca sahip olduğu rol kapsamında izin verilen işlemleri gerçekleştirebilmelidir.
- Yetkisiz işlemlere erişim engellenmelidir.
- Kullanıcı yetkileri sistemde tanımlanan roller üzerinden değerlendirilmelidir.
- Kimliği doğrulanmamış kullanıcılar yetkilendirme gerektiren sistem fonksiyonlarına erişememelidir.

### İlgili Gereksinimler

- BR-06
- BRULE-25
- BRULE-28
- NFR-02
- NFR-03

---

## US-24 - Yönetim İşlemlerinin Yetkisiz Kullanıcılardan Korunması

### Kullanıcı Hikayesi

Bir site yöneticisi olarak, yönetim yetkisi gerektiren işlemlerin yetkisiz kullanıcılar tarafından gerçekleştirilememesini istiyorum; böylece yönetim kayıtlarının kontrollü şekilde yönetilmesini sağlayabilirim.

### Kabul Kriterleri

- Site sakinleri yönetim yetkisi gerektiren kayıtları oluşturamamalıdır.
- Site sakinleri yönetim yetkisi gerektiren kayıtları güncelleyememelidir.
- Yetkisiz işlem girişimleri sistem tarafından engellenmelidir.
- Kullanıcının erişim yetkisi ilgili işlem gerçekleştirilmeden önce kontrol edilmelidir.

### İlgili Gereksinimler

- BR-06
- BRULE-26
- NFR-02
- NFR-11

---

## US-25 - Özel Kullanıcı Bilgilerinin Korunması

### Kullanıcı Hikayesi

Bir site sakini olarak, diğer site sakinlerine ait özel bilgilere erişememek ve kendi özel bilgilerimin yetkisiz kullanıcılar tarafından görüntülenmemesini istiyorum; böylece kullanıcı bilgilerinin gizliliği korunabilir.

### Kabul Kriterleri

- Site sakini başka site sakinlerine ait özel bilgilere erişememelidir.
- Kullanıcıların veri erişimi sahip oldukları rol ve yetkiler kapsamında sınırlandırılmalıdır.
- Yetkisiz kullanıcılar özel kullanıcı bilgilerini görüntüleyememelidir.
- Daire ve finansal bilgilere erişim ilgili kullanıcılar ve yetkili yönetim kullanıcıları ile sınırlandırılmalıdır.

### İlgili Gereksinimler

- BR-06
- BRULE-27
- NFR-11
- NFR-12

---

## Kullanıcı Hikayesi Özeti

| Kullanıcı Hikayesi | Rol | Amaç |
|---|---|---|
| US-23 | Sistem Kullanıcısı | Rol kapsamında izin verilen işlemlere erişmek |
| US-24 | Site Yöneticisi | Yönetim işlemlerini yetkisiz erişime karşı korumak |
| US-25 | Site Sakini | Özel kullanıcı bilgilerinin gizliliğini korumak |

---

## Genel Değerlendirme

Kullanıcı yetkilendirme kullanıcı hikayeleri, sistem kullanıcılarının sahip oldukları roller kapsamında işlem gerçekleştirmesi ve yetkisiz işlem veya veri erişimlerinin engellenmesi temel alınarak hazırlanmıştır.

Tanımlanan kabul kriterleri, kullanıcı hikayelerinin tamamlanma koşullarının değerlendirilmesinde referans olarak kullanılacaktır.
