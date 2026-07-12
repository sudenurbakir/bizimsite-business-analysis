# BizimSite - Rol ve Yetki Matrisi

BizimSite içerisinde kullanıcıların gerçekleştirebileceği işlemler sahip oldukları rol ve sorumluluklara göre sınırlandırılmıştır.

Rol ve Yetki Matrisi, sistem içerisindeki kullanıcı rollerini ve bu rollerin temel süreçler üzerindeki yetkilerini tanımlamaktadır.

---

## Kullanıcı Rolleri

BizimSite kapsamında aşağıdaki temel kullanıcı rolleri belirlenmiştir:

- Site Yöneticisi
- Site Sakini
- Muhasebe Sorumlusu
- Teknik Ekip

---

## Rol ve Yetki Matrisi

| İşlem | Site Yöneticisi | Site Sakini | Muhasebe Sorumlusu | Teknik Ekip |
|---|---|---|---|---|
| Aidat bilgilerini görüntüleme | Tümü | Kendi dairesi | Tümü | Yetki Yok |
| Aidat kaydı oluşturma | Yetkili | Yetki Yok | Yetkili | Yetki Yok |
| Aidat kaydı güncelleme | Yetkili | Yetki Yok | Yetkili | Yetki Yok |
| Duyuru görüntüleme | Yetkili | Yetkili | Yetkili | Yetkili |
| Duyuru oluşturma | Yetkili | Yetki Yok | Yetki Yok | Yetki Yok |
| Duyuru yayımlama | Yetkili | Yetki Yok | Yetki Yok | Yetki Yok |
| Arıza talebi oluşturma | Yetkili | Yetkili | Yetki Yok | Yetki Yok |
| Arıza taleplerini görüntüleme | Tümü | Kendi talepleri | Yetki Yok | Atanan talepler |
| Arıza durumu güncelleme | Yetkili | Yetki Yok | Yetki Yok | Atanan talepler |
| Ortak alan uygunluğunu görüntüleme | Yetkili | Yetkili | Yetkili | Yetkili |
| Rezervasyon oluşturma | Yetkili | Yetkili | Yetki Yok | Yetki Yok |
| Ortak gider görüntüleme | Yetkili | Yayımlanan kayıtlar | Yetkili | Yetki Yok |
| Ortak gider oluşturma | Yetkili | Yetki Yok | Yetkili | Yetki Yok |
| Ortak gider güncelleme | Yetkili | Yetki Yok | Yetkili | Yetki Yok |

---

## Rol Açıklamaları

### Site Yöneticisi

Site yönetim süreçlerinden sorumlu ana operasyonel kullanıcıdır.

Aidat, duyuru, arıza talepleri, rezervasyonlar ve ortak gider süreçlerini yönetebilir.

---

### Site Sakini

Apartman veya sitede bulunan bir daire ile ilişkili son kullanıcıdır.

Kendi dairesine ait aidat bilgilerini görüntüleyebilir, duyurulara erişebilir, arıza talebi oluşturabilir ve ortak alan rezervasyonu gerçekleştirebilir.

Site sakini başka dairelere veya kullanıcılara ait özel bilgilere erişemez.

---

### Muhasebe Sorumlusu

Aidat ve ortak gider süreçlerinin finansal takibinden sorumlu kullanıcıdır.

Aidat kayıtlarını ve ortak gider bilgilerini oluşturabilir, görüntüleyebilir ve güncelleyebilir.

Yönetimsel veya teknik süreçler üzerinde işlem yetkisi bulunmamaktadır.

---

### Teknik Ekip

Kendisine yönlendirilen arıza ve hizmet taleplerinin yürütülmesinden sorumludur.

Yalnızca kendisine atanan talepleri görüntüleyebilir ve bu taleplerin durumlarını güncelleyebilir.

Finansal ve yönetimsel bilgilere erişim yetkisi bulunmamaktadır.

---

## Yetkilendirme Yaklaşımı

BizimSite içerisinde rol tabanlı yetkilendirme yaklaşımı kullanılacaktır.

Her kullanıcı sistemde tanımlanan bir role sahip olacak ve yalnızca ilgili rol için izin verilen işlemleri gerçekleştirebilecektir.

Kullanıcıların görev alanı dışında kalan bilgilere ve işlemlere erişimi sınırlandırılacaktır.

---

## Genel Değerlendirme

Rol ve Yetki Matrisi ile BizimSite içerisindeki temel kullanıcı rollerinin sorumlulukları ve sistem yetkileri netleştirilmiştir.

Belirlenen yetkiler, fonksiyonel gereksinimlerin ve kullanıcı hikâyelerinin oluşturulmasında referans olarak kullanılacaktır.
