# BizimSite - Alan Kısıtları ve Doğrulama Kuralları

BizimSite sisteminde kullanılan temel veri alanlarının geçerli ve tutarlı bilgiler içermesini sağlamak amacıyla alan kısıtları ve doğrulama kuralları tanımlanmıştır.

Bu kurallar, geçersiz veya eksik verilerin sistem kayıtlarına eklenmesini önlemeyi amaçlamaktadır.

---

## Kullanıcı Alanları

* Kullanıcı adı ve soyadı boş bırakılamaz.
* E-posta bilgisi boş bırakılamaz.
* E-posta bilgisi geçerli bir e-posta formatında olmalıdır.
* Aynı e-posta adresi birden fazla kullanıcı hesabı için kullanılamaz.
* Kullanıcı rolü sistemde tanımlanan rollerden biri olmalıdır.

---

## Daire Alanları

* Blok bilgisi boş bırakılamaz.
* Daire numarası boş bırakılamaz.
* Aynı blok içerisinde aynı daire numarası birden fazla daire kaydı için kullanılamaz.

---

## Aidat Alanları

* Aidat kaydı bir daire ile ilişkilendirilmelidir.
* Aidat dönemi boş bırakılamaz.
* Aidat tutarı sıfırdan büyük olmalıdır.
* Ödeme durumu "Ödendi" veya "Ödenmedi" değerlerinden biri olmalıdır.
* Aynı daire ve aynı aidat dönemi için birden fazla aidat kaydı oluşturulmamalıdır.

---

## Duyuru Alanları

* Duyuru başlığı boş bırakılamaz.
* Duyuru içeriği boş bırakılamaz.
* Duyuru durumu "Taslak" veya "Yayımlandı" değerlerinden biri olmalıdır.
* Yayımlanan duyurunun yayımlanma tarihi bulunmalıdır.

---

## Talep Alanları

* Talep, talebi oluşturan kullanıcı ile ilişkilendirilmelidir.
* Talep türü boş bırakılamaz.
* Talep açıklaması boş bırakılamaz.
* Talep durumu "Yeni", "İşlemde" veya "Tamamlandı" değerlerinden biri olmalıdır.
* Talep oluşturma tarihi kayıt altına alınmalıdır.

---

## Ortak Alan Alanları

* Ortak alan adı boş bırakılamaz.
* Rezervasyona açık bilgisi yalnızca doğru veya yanlış değerlerinden birini almalıdır.

---

## Rezervasyon Alanları

* Rezervasyon, rezervasyonu oluşturan kullanıcı ile ilişkilendirilmelidir.
* Rezervasyon bir ortak alan ile ilişkilendirilmelidir.
* Başlangıç ve bitiş tarihleri boş bırakılamaz.
* Bitiş tarihi başlangıç tarihinden sonra olmalıdır.
* Geçmiş tarihli bir zaman aralığı için yeni rezervasyon oluşturulmamalıdır.
* Rezervasyon durumu "Aktif", "İptal Edildi" veya "Tamamlandı" değerlerinden biri olmalıdır.
* Aynı ortak alan için çakışan zaman aralıklarında birden fazla aktif rezervasyon oluşturulmamalıdır.

---

## Ortak Gider Alanları

* Gider türü boş bırakılamaz.
* Gider dönemi boş bırakılamaz.
* Gider tutarı sıfırdan büyük olmalıdır.
* Ortak gider durumu "Yayımlanmadı" veya "Yayımlandı" değerlerinden biri olmalıdır.
* Bireysel dairelere ait elektrik, su veya doğalgaz faturaları ortak gider olarak kaydedilmemelidir.

---

## Genel Değerlendirme

Alan kısıtları ve doğrulama kuralları, BizimSite sisteminde tutulan verilerin geçerli, tutarlı ve iş kurallarına uygun olmasını sağlamaya yönelik temel kontrolleri tanımlamaktadır.

Bu kurallar, veritabanı tasarımı ve sistem geliştirme süreçlerinde veri doğrulama mekanizmalarının oluşturulmasında referans olarak kullanılacaktır.
