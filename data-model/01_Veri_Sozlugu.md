# BizimSite - Veri Sözlüğü

BizimSite sisteminde yer alan temel veri varlıkları ve bu varlıklara ait alanlar aşağıdaki veri sözlüğünde tanımlanmıştır.

Veri sözlüğü, sistem veri modelinde kullanılan alanların amaçlarını ve temel veri özelliklerini açıklamaktadır.

---

## 1. Kullanıcı

Sisteme erişen kullanıcıların temel bilgilerini temsil eder.

| Alan         | Veri Türü | Anahtar | Açıklama                                                            |
| ------------ | --------- | ------- | ------------------------------------------------------------------- |
| kullanici_id | int       | PK      | Kullanıcı kaydını benzersiz olarak tanımlar.                        |
| ad           | string    | -       | Kullanıcının ad bilgisini tutar.                                    |
| soyad        | string    | -       | Kullanıcının soyad bilgisini tutar.                                 |
| eposta       | string    | -       | Kullanıcının sisteme kayıtlı e-posta adresini tutar.                |
| parola       | string    | -       | Kullanıcının güvenli şekilde saklanan parola bilgisini temsil eder. |
| rol          | string    | -       | Kullanıcının sistem içerisindeki rol bilgisini tutar.               |

---

## 2. Daire

Site içerisinde bulunan daire kayıtlarını temsil eder.

| Alan     | Veri Türü | Anahtar | Açıklama                                 |
| -------- | --------- | ------- | ---------------------------------------- |
| daire_id | int       | PK      | Daire kaydını benzersiz olarak tanımlar. |
| blok     | string    | -       | Dairenin bulunduğu blok bilgisini tutar. |
| daire_no | string    | -       | Dairenin numara bilgisini tutar.         |

---

## 3. Aidat

Dairelere ait dönemsel aidat kayıtlarını ve ödeme durumlarını temsil eder.

| Alan         | Veri Türü | Anahtar | Açıklama                                         |
| ------------ | --------- | ------- | ------------------------------------------------ |
| aidat_id     | int       | PK      | Aidat kaydını benzersiz olarak tanımlar.         |
| daire_id     | int       | FK      | Aidat kaydının ilişkili olduğu daireyi belirtir. |
| donem        | string    | -       | Aidat kaydının ait olduğu dönemi belirtir.       |
| tutar        | decimal   | -       | Aidat tutarını belirtir.                         |
| odeme_durumu | string    | -       | Aidat kaydının ödeme durumunu belirtir.          |

### Ödeme Durumu Değerleri

* Ödendi
* Ödenmedi

---

## 4. Duyuru

Site yönetimi tarafından oluşturulan duyuru kayıtlarını temsil eder.

| Alan                   | Veri Türü | Anahtar | Açıklama                                              |
| ---------------------- | --------- | ------- | ----------------------------------------------------- |
| duyuru_id              | int       | PK      | Duyuru kaydını benzersiz olarak tanımlar.             |
| olusturan_kullanici_id | int       | FK      | Duyuruyu oluşturan kullanıcıyı belirtir.              |
| baslik                 | string    | -       | Duyurunun başlık bilgisini tutar.                     |
| icerik                 | string    | -       | Duyuru içeriğini tutar.                               |
| durum                  | string    | -       | Duyurunun mevcut durumunu belirtir.                   |
| yayimlanma_tarihi      | datetime  | -       | Duyurunun yayımlandığı tarih ve saat bilgisini tutar. |

### Durum Değerleri

* Taslak
* Yayımlandı

---

## 5. Talep

Site sakinleri tarafından oluşturulan arıza ve hizmet taleplerini temsil eder.

| Alan             | Veri Türü | Anahtar | Açıklama                                             |
| ---------------- | --------- | ------- | ---------------------------------------------------- |
| talep_id         | int       | PK      | Talep kaydını benzersiz olarak tanımlar.             |
| kullanici_id     | int       | FK      | Talebi oluşturan kullanıcıyı belirtir.               |
| talep_turu       | string    | -       | Talebin arıza veya hizmet talebi türünü belirtir.    |
| aciklama         | string    | -       | Talebe ilişkin açıklama bilgisini tutar.             |
| durum            | string    | -       | Talebin mevcut durumunu belirtir.                    |
| olusturma_tarihi | datetime  | -       | Talebin oluşturulduğu tarih ve saat bilgisini tutar. |

### Durum Değerleri

* Yeni
* İşlemde
* Tamamlandı

---

## 6. Ortak Alan

Rezervasyon işlemine konu olabilecek ortak kullanım alanlarını temsil eder.

| Alan              | Veri Türü | Anahtar | Açıklama                                                         |
| ----------------- | --------- | ------- | ---------------------------------------------------------------- |
| ortak_alan_id     | int       | PK      | Ortak alan kaydını benzersiz olarak tanımlar.                    |
| ad                | string    | -       | Ortak alanın ad bilgisini tutar.                                 |
| rezervasyona_acik | boolean   | -       | Ortak alanın rezervasyon işlemine açık olup olmadığını belirtir. |

---

## 7. Rezervasyon

Site sakinlerinin ortak alanlar için oluşturduğu rezervasyon kayıtlarını temsil eder.

| Alan             | Veri Türü | Anahtar | Açıklama                                             |
| ---------------- | --------- | ------- | ---------------------------------------------------- |
| rezervasyon_id   | int       | PK      | Rezervasyon kaydını benzersiz olarak tanımlar.       |
| kullanici_id     | int       | FK      | Rezervasyonu oluşturan kullanıcıyı belirtir.         |
| ortak_alan_id    | int       | FK      | Rezervasyonun ilişkili olduğu ortak alanı belirtir.  |
| baslangic_tarihi | datetime  | -       | Rezervasyon başlangıç tarih ve saat bilgisini tutar. |
| bitis_tarihi     | datetime  | -       | Rezervasyon bitiş tarih ve saat bilgisini tutar.     |
| durum            | string    | -       | Rezervasyonun mevcut durumunu belirtir.              |

### Durum Değerleri

* Aktif
* İptal Edildi
* Tamamlandı

---

## 8. Ortak Gider

Site veya apartmana ait ortak kullanım giderlerini temsil eder.

| Alan           | Veri Türü | Anahtar | Açıklama                                           |
| -------------- | --------- | ------- | -------------------------------------------------- |
| ortak_gider_id | int       | PK      | Ortak gider kaydını benzersiz olarak tanımlar.     |
| gider_turu     | string    | -       | Ortak giderin tür bilgisini tutar.                 |
| donem          | string    | -       | Ortak giderin ait olduğu dönemi belirtir.          |
| tutar          | decimal   | -       | Ortak gider tutarını belirtir.                     |
| durum          | string    | -       | Ortak gider kaydının yayımlanma durumunu belirtir. |

### Durum Değerleri

* Yayımlanmadı
* Yayımlandı

---

## Anahtar Açıklamaları

**PK (Primary Key):** Bir kaydı sistem içerisinde benzersiz olarak tanımlayan alanı ifade eder.

**FK (Foreign Key):** Bir veri varlığının başka bir veri varlığı ile ilişkisini sağlayan alanı ifade eder.

---

## Genel Değerlendirme

Veri sözlüğü, BizimSite sisteminde kullanılacak temel veri varlıklarının alanlarını, veri türlerini ve kullanım amaçlarını açıklamaktadır.

Tanımlanan alanlar, veritabanı tasarımının detaylandırılması ve sistem geliştirme çalışmalarında referans olarak kullanılacaktır.
