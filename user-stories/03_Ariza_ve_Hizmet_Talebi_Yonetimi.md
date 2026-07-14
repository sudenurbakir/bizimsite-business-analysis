# BizimSite - Arıza ve Hizmet Talebi Yönetimi Kullanıcı Hikayeleri

BizimSite arıza ve hizmet talebi yönetimi süreci kapsamında kullanıcı ihtiyaçlarını sistem davranışlarına dönüştürmek amacıyla kullanıcı hikayeleri hazırlanmıştır.

Her kullanıcı hikayesi, ilgili kullanıcının hedefini ve bu hedef sonucunda elde etmek istediği değeri açıklamaktadır.

---

## US-09 - Arıza veya Hizmet Talebi Oluşturma

### Kullanıcı Hikayesi

Bir site sakini olarak, yaşadığım arıza veya hizmet ihtiyacı için talep oluşturmak istiyorum; böylece ilgili sorunun site yönetimine iletilmesini sağlayabilirim.

### Kabul Kriterleri

- Site sakini yeni arıza veya hizmet talebi oluşturabilmelidir.
- Talep, talebi oluşturan kullanıcı ile ilişkilendirilmelidir.
- Talep açıklama bilgisi içermelidir.
- Zorunlu alanlar tamamlanmadan talep oluşturulmamalıdır.
- Yeni oluşturulan talep "Yeni" durumuyla kayıt altına alınmalıdır.
- Başarılı kayıt işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-03
- FR-13
- FR-14
- FR-15
- NFR-11
- NFR-18

---

## US-10 - Talebi Teknik Ekibe Yönlendirme

### Kullanıcı Hikayesi

Bir site yöneticisi olarak, oluşturulan arıza veya hizmet talebini teknik ekip personeline yönlendirmek istiyorum; böylece talebin ilgili personel tarafından işleme alınmasını sağlayabilirim.

### Kabul Kriterleri

- Site yöneticisi oluşturulan talepleri görüntüleyebilmelidir.
- Site yöneticisi bir talebi teknik ekip personeline yönlendirebilmelidir.
- Talep, seçilen teknik ekip personeli ile ilişkilendirilmelidir.
- Yetkisiz kullanıcılar talepleri teknik ekip personeline yönlendirememelidir.
- Başarılı yönlendirme işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-03
- FR-16
- FR-44
- NFR-02
- NFR-11

---

## US-11 - Atanan Talepleri Görüntüleme

### Kullanıcı Hikayesi

Bir teknik ekip personeli olarak, yalnızca bana atanan arıza ve hizmet taleplerini görüntülemek istiyorum; böylece sorumlu olduğum işleri takip edebilirim.

### Kabul Kriterleri

- Teknik ekip personeli kendisine atanan talepleri görüntüleyebilmelidir.
- Teknik ekip personeli kendisine atanmamış talepleri görüntüleyememelidir.
- Talebin açıklaması ve mevcut durumu görüntülenebilmelidir.
- Talep listesi tanımlanan kullanım koşulları altında en fazla 3 saniye içerisinde görüntülenmelidir.

### İlgili Gereksinimler

- BR-03
- FR-17
- FR-43
- NFR-05
- NFR-12

---

## US-12 - Talep Durumunu Güncelleme

### Kullanıcı Hikayesi

Bir teknik ekip personeli olarak, bana atanan talebin durumunu güncellemek istiyorum; böylece talebin mevcut işlem aşaması sistem üzerinden takip edilebilir.

### Kabul Kriterleri

- Teknik ekip personeli yalnızca kendisine atanan taleplerin durumunu güncelleyebilmelidir.
- Talep durumları "Yeni", "İşlemde" ve "Tamamlandı" sırasına göre ilerlemelidir.
- "Yeni" durumundaki bir talep doğrudan "Tamamlandı" durumuna geçirilememelidir.
- Tanımlı olmayan bir durum değeri kaydedilmemelidir.
- Teknik ekip personeli kendisine atanmamış bir talebin durumunu güncelleyememelidir.
- Başarılı güncelleme işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-03
- BRULE-16
- FR-18
- FR-19
- FR-43
- NFR-11
- NFR-19

---

## US-13 - Kendi Taleplerinin Durumunu Görüntüleme

### Kullanıcı Hikayesi

Bir site sakini olarak, oluşturduğum arıza ve hizmet taleplerinin güncel durumunu görüntülemek istiyorum; böylece talebimin hangi aşamada olduğunu takip edebilirim.

### Kabul Kriterleri

- Site sakini kendi oluşturduğu talepleri görüntüleyebilmelidir.
- Talebin güncel durumu görüntülenebilmelidir.
- Site sakini başka kullanıcılar tarafından oluşturulan özel talep kayıtlarına erişememelidir.
- Talep bilgileri tanımlanan kullanım koşulları altında en fazla 3 saniye içerisinde görüntülenmelidir.

### İlgili Gereksinimler

- BR-03
- FR-20
- NFR-05
- NFR-12

---

## US-14 - Geçmiş Talepleri Görüntüleme

### Kullanıcı Hikayesi

Bir site yöneticisi olarak, geçmiş arıza ve hizmet taleplerini görüntülemek istiyorum; böylece daha önce oluşturulan talepleri ve tamamlanan işlemleri takip edebilirim.

### Kabul Kriterleri

- Site yöneticisi geçmiş arıza ve hizmet taleplerini görüntüleyebilmelidir.
- Tamamlanmış talepler geçmiş talep kayıtları içerisinde görüntülenebilmelidir.
- Talebin mevcut durumu görüntülenebilmelidir.
- Geçmiş talep listesi tanımlanan kullanım koşulları altında en fazla 3 saniye içerisinde görüntülenmelidir.

### İlgili Gereksinimler

- BR-03
- FR-21
- NFR-05

---

## Kullanıcı Hikayesi Özeti

| Kullanıcı Hikayesi | Rol | Amaç |
|---|---|---|
| US-09 | Site Sakini | Arıza veya hizmet talebi oluşturmak |
| US-10 | Site Yöneticisi | Talebi teknik ekibe yönlendirmek |
| US-11 | Teknik Ekip | Atanan talepleri görüntülemek |
| US-12 | Teknik Ekip | Talep durumunu güncellemek |
| US-13 | Site Sakini | Kendi taleplerinin durumunu takip etmek |
| US-14 | Site Yöneticisi | Geçmiş talepleri görüntülemek |

---

## Genel Değerlendirme

Arıza ve hizmet talebi yönetimi kullanıcı hikayeleri, site sakinlerinin talep oluşturması, site yöneticisinin talepleri teknik ekibe yönlendirmesi ve teknik ekip personelinin atanan talepleri yönetmesi temel alınarak hazırlanmıştır.

Tanımlanan kabul kriterleri, kullanıcı hikayelerinin tamamlanma koşullarının değerlendirilmesinde referans olarak kullanılacaktır.
