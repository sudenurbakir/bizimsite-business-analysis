# BizimSite - Ortak Alan Rezervasyonu Kullanıcı Hikayeleri

BizimSite ortak alan rezervasyonu süreci kapsamında kullanıcı ihtiyaçlarını sistem davranışlarına dönüştürmek amacıyla kullanıcı hikayeleri hazırlanmıştır.

Her kullanıcı hikayesi, ilgili kullanıcının hedefini ve bu hedef sonucunda elde etmek istediği değeri açıklamaktadır.

---

## US-15 - Rezervasyona Açık Ortak Alanları Görüntüleme

### Kullanıcı Hikayesi

Bir site sakini olarak, rezervasyona açık ortak alanları görüntülemek istiyorum; böylece rezervasyon oluşturabileceğim alanları görebilirim.

### Kabul Kriterleri

- Site sakini rezervasyona açık ortak alanları görüntüleyebilmelidir.
- Rezervasyona kapalı ortak alanlar için rezervasyon işlemi başlatılamamalıdır.
- Ortak alan bilgileri kullanıcı tarafından görüntülenebilmelidir.

### İlgili Gereksinimler

- BR-04
- BRULE-14

---

## US-16 - Ortak Alan Rezervasyonu Oluşturma

### Kullanıcı Hikayesi

Bir site sakini olarak, rezervasyona açık bir ortak alan için rezervasyon oluşturmak istiyorum; böylece ortak alanı belirlediğim tarih ve saat aralığında kullanabilirim.

### Kabul Kriterleri

- Site sakini rezervasyona açık bir ortak alan için rezervasyon oluşturabilmelidir.
- Rezervasyon tarih ve saat aralığı bilgilerini içermelidir.
- Rezervasyon, rezervasyonu oluşturan kullanıcı ile ilişkilendirilmelidir.
- Geçmiş tarihli bir zaman aralığı için rezervasyon oluşturulamamalıdır.
- Zorunlu alanlar tamamlanmadan rezervasyon oluşturulmamalıdır.
- Başarılı rezervasyon işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-04
- BRULE-14
- BRULE-16
- BRULE-17
- NFR-11
- NFR-18

---

## US-17 - Çakışan Rezervasyonun Engellenmesi

### Kullanıcı Hikayesi

Bir site sakini olarak, seçtiğim ortak alan için uygun bir tarih ve saat aralığında rezervasyon oluşturmak istiyorum; böylece aynı zaman aralığında birden fazla aktif rezervasyon oluşmasından kaynaklanan kullanım çakışmaları önlenebilir.

### Kabul Kriterleri

- Sistem, aynı ortak alan için mevcut aktif rezervasyonları kontrol etmelidir.
- Aynı tarih ve saat aralığı ile çakışan aktif bir rezervasyon bulunması durumunda yeni rezervasyon oluşturulmamalıdır.
- Başarısız rezervasyon işlemi sonrasında kullanıcıya anlaşılır bir hata mesajı gösterilmelidir.
- Çakışmayan tarih ve saat aralıkları için rezervasyon oluşturulabilmelidir.

### İlgili Gereksinimler

- BR-04
- BRULE-15
- NFR-10
- NFR-18

---

## US-18 - Kendi Rezervasyonlarını Görüntüleme

### Kullanıcı Hikayesi

Bir site sakini olarak, oluşturduğum ortak alan rezervasyonlarını görüntülemek istiyorum; böylece rezervasyon bilgilerimi takip edebilirim.

### Kabul Kriterleri

- Site sakini kendi oluşturduğu rezervasyon kayıtlarını görüntüleyebilmelidir.
- Rezervasyonun ortak alan, tarih ve saat bilgileri görüntülenebilmelidir.
- Site sakini başka kullanıcıların özel rezervasyon kayıtlarına erişememelidir.
- Rezervasyon bilgileri tanımlanan kullanım koşulları altında en fazla 3 saniye içerisinde görüntülenmelidir.

### İlgili Gereksinimler

- BR-04
- BRULE-18
- NFR-05
- NFR-12

---

## US-19 - Rezervasyon İptal Etme

### Kullanıcı Hikayesi

Bir site sakini olarak, oluşturduğum ve henüz gerçekleşmemiş bir rezervasyonu iptal etmek istiyorum; böylece kullanmayacağım ortak alan rezervasyonunu iptal edebilirim.

### Kabul Kriterleri

- Site sakini yalnızca kendi oluşturduğu rezervasyonları iptal edebilmelidir.
- Henüz gerçekleşmemiş rezervasyonlar iptal edilebilmelidir.
- Geçmiş rezervasyonlar iptal edilememelidir.
- Başka kullanıcılar tarafından oluşturulan rezervasyonlar iptal edilememelidir.
- Başarılı iptal işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

### İlgili Gereksinimler

- BR-04
- BRULE-19
- NFR-10
- NFR-11

---

## Kullanıcı Hikayesi Özeti

| Kullanıcı Hikayesi | Rol | Amaç |
|---|---|---|
| US-15 | Site Sakini | Rezervasyona açık ortak alanları görüntülemek |
| US-16 | Site Sakini | Ortak alan rezervasyonu oluşturmak |
| US-17 | Site Sakini | Çakışmayan zaman aralığında rezervasyon oluşturmak |
| US-18 | Site Sakini | Kendi rezervasyonlarını görüntülemek |
| US-19 | Site Sakini | Kendi rezervasyonunu iptal etmek |

---

## Genel Değerlendirme

Ortak alan rezervasyonu kullanıcı hikayeleri, site sakinlerinin rezervasyona açık ortak alanları görüntülemesi, uygun tarih ve saat aralıkları için rezervasyon oluşturması, kendi rezervasyon kayıtlarını takip etmesi ve henüz gerçekleşmemiş rezervasyonlarını iptal etmesi temel alınarak hazırlanmıştır.

Tanımlanan kabul kriterleri, kullanıcı hikayelerinin tamamlanma koşullarının değerlendirilmesinde referans olarak kullanılacaktır.
