# BizimSite - Fonksiyonel Gereksinimler

BizimSite sisteminin kullanıcı ihtiyaçlarını ve tanımlanan iş gereksinimlerini karşılayabilmesi için gerekli temel sistem fonksiyonları aşağıda tanımlanmıştır.

Fonksiyonel gereksinimler, sistemin kullanıcılar için hangi işlevleri sağlaması gerektiğini belirtmektedir.

---

## 1. Aidat Yönetimi

**İlgili İş Gereksinimi:** BR-01

### FR-01

Sistem, yetkili kullanıcının yeni aidat kaydı oluşturmasına izin vermelidir.

### FR-02

Sistem, aidat kaydının bir daire ve aidat dönemi ile ilişkilendirilmesini sağlamalıdır.

### FR-03

Sistem, yetkili kullanıcının aidat ödeme durumunu güncellemesine izin vermelidir.

### FR-04

Sistem, site sakininin yalnızca kendi dairesine ait aidat bilgilerini görüntülemesini sağlamalıdır.

### FR-05

Sistem, site yöneticisi ve muhasebe sorumlusunun aidat kayıtlarını görüntülemesine izin vermelidir.

---

## 2. Duyuru Yönetimi

**İlgili İş Gereksinimi:** BR-02

### FR-07

Sistem, oluşturulan duyurunun taslak olarak kaydedilebilmesini sağlamalıdır.

### FR-08

Sistem, site yöneticisinin taslak durumundaki bir duyuruyu görüntülemesine ve düzenlemesine izin vermelidir.

### FR-09

Sistem, site yöneticisinin bir duyuruyu yayımlamasına izin vermelidir.

### FR-10

Sistem, site sakinlerinin yalnızca yayımlanmış duyuruları görüntülemesini sağlamalıdır.

### FR-11

Sistem, yayımlanan duyuruların yayımlanma tarihini kayıt altına almalıdır.

### FR-12

Sistem, kullanıcıların geçmiş yayımlanmış duyuruları görüntülemesini sağlamalıdır.

---

## 3. Arıza ve Hizmet Talebi Yönetimi

**İlgili İş Gereksinimi:** BR-03

### FR-13

Sistem, site sakininin yeni arıza veya hizmet talebi oluşturmasına izin vermelidir.

### FR-14

Sistem, oluşturulan talebi ilgili kullanıcı ile ilişkilendirmelidir.

### FR-15

Sistem, yeni oluşturulan talepleri "Yeni" durumuyla kayıt altına almalıdır.

### FR-16

Sistem, yetkili kullanıcının bir talebi teknik ekip personeline yönlendirmesine izin vermelidir.

### FR-17

Sistem, teknik ekip personelinin yalnızca kendisine atanan talepleri görüntülemesini sağlamalıdır.

### FR-18

Sistem, teknik ekip personelinin kendisine atanan talebin durumunu güncellemesine izin vermelidir.

### FR-19

Sistem, talep durumlarının "Yeni", "İşlemde" veya "Tamamlandı" değerlerinden biri olmasını sağlamalıdır.

### FR-20

Sistem, site sakininin kendi oluşturduğu taleplerin güncel durumunu görüntülemesini sağlamalıdır.

### FR-21

Sistem, geçmiş arıza ve hizmet taleplerinin görüntülenebilmesini sağlamalıdır.

---

## 4. Ortak Alan Rezervasyon Yönetimi

**İlgili İş Gereksinimi:** BR-04

### FR-22

Sistem, rezervasyona açık ortak alanların görüntülenmesini sağlamalıdır.

### FR-23

Sistem, ortak alanların tarih ve saat bazlı uygunluk durumunu görüntülemelidir.

### FR-24

Sistem, site sakininin uygun bir tarih ve saat aralığı için rezervasyon oluşturmasına izin vermelidir.

### FR-25

Sistem, rezervasyon oluşturulmadan önce aynı ortak alan, tarih ve saat aralığında aktif rezervasyon bulunup bulunmadığını kontrol etmelidir.

### FR-26

Sistem, çakışan bir aktif rezervasyon bulunması durumunda yeni rezervasyon oluşturulmasını engellemelidir.

### FR-27

Sistem, oluşturulan rezervasyonu ilgili kullanıcı ile ilişkilendirmelidir.

### FR-28

Sistem, site sakininin kendi rezervasyon kayıtlarını görüntülemesini sağlamalıdır.

### FR-29

Sistem, geçmiş tarihli bir zaman aralığı için yeni rezervasyon oluşturulmasını engellemelidir.

---

## 5. Ortak Gider Yönetimi

**İlgili İş Gereksinimi:** BR-05

### FR-30

Sistem, yetkili kullanıcının yeni ortak gider kaydı oluşturmasına izin vermelidir.

### FR-31

Sistem, ortak gider kaydının gider türü, dönem ve tutar bilgilerini içermesini sağlamalıdır.

### FR-32

Sistem, yetkili kullanıcının ortak gider kaydını güncellemesine izin vermelidir.

### FR-33

Sistem, yetkili kullanıcının ortak gider kaydını yayımlamasına izin vermelidir.

### FR-34

Sistem, site sakinlerinin yalnızca yayımlanmış ortak gider kayıtlarını görüntülemesini sağlamalıdır.

### FR-35

Sistem, yayımlanmamış ortak gider kayıtlarının site sakinleri tarafından görüntülenmesini engellemelidir.

### FR-36

Sistem, geçmiş dönem ortak gider kayıtlarının görüntülenebilmesini sağlamalıdır.

---

## 6. Kullanıcı ve Yetkilendirme Yönetimi

**İlgili İş Gereksinimi:** BR-06

### FR-37

Sistem, site yöneticisinin yeni kullanıcı hesabı oluşturmasına izin vermelidir.

### FR-38

Sistem, site yöneticisinin oluşturulan kullanıcı hesabını tanımlı bir kullanıcı rolü ile ilişkilendirmesine izin vermelidir.

### FR-39

Sistem, site sakini rolüne sahip kullanıcıların ilgili daire ile ilişkilendirilmesini sağlamalıdır.

### FR-40

Sistem, kullanıcıların sisteme giriş yapmasını sağlamalıdır.

### FR-41

Sistem, kullanıcıların yalnızca sahip oldukları rol kapsamında izin verilen işlemleri gerçekleştirmesini sağlamalıdır.

### FR-42

Sistem, site sakinlerinin başka dairelere ait özel bilgileri görüntülemesini engellemelidir.

### FR-43

Sistem, teknik ekip personelinin kendisine atanmamış taleplere erişmesini engellemelidir.

### FR-44

Sistem, yönetim yetkisi gerektiren işlemlerin yetkisiz kullanıcılar tarafından gerçekleştirilmesini engellemelidir.
---

## Fonksiyonel Gereksinim Özeti

| İş Gereksinimi | Fonksiyonel Gereksinimler |
|---|---|
| BR-01 - Aidat Takibi | FR-01 - FR-05 |
| BR-02 - Duyuru Yönetimi | FR-06 - FR-11 |
| BR-03 - Arıza ve Hizmet Talepleri | FR-12 - FR-20 |
| BR-04 - Ortak Alan Rezervasyonu | FR-21 - FR-28 |
| BR-05 - Ortak Gider Yönetimi | FR-29 - FR-35 |
| BR-06 - Kullanıcı Yetkilendirme | FR-36 - FR-43 |

---

## Genel Değerlendirme

Tanımlanan fonksiyonel gereksinimler, BizimSite sisteminin ilk sürümünde sağlaması beklenen temel sistem davranışlarını açıklamaktadır.

Bu gereksinimler, kullanıcı hikâyelerinin, kabul kriterlerinin ve gereksinim izlenebilirlik matrisinin oluşturulmasında referans olarak kullanılacaktır.
