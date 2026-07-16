# BizimSite - API Genel Bakış

BizimSite sistemi, istemci uygulamaları ile sunucu arasındaki veri alışverişini REST API yaklaşımı ile gerçekleştirecektir.

API tasarımı, sistemde yer alan temel iş süreçlerini destekleyecek şekilde planlanmıştır.

---

## API Amaçları

API katmanı aşağıdaki temel işlemleri desteklemektedir:

* Kullanıcı kimlik doğrulama
* Aidat bilgilerini görüntüleme
* Duyuru yönetimi
* Arıza ve hizmet taleplerinin yönetimi
* Ortak alan rezervasyonu işlemleri
* Ortak gider yönetimi

---

## API Kaynakları

Sistem aşağıdaki temel kaynaklar üzerinden hizmet sunacaktır.

| Kaynak      | Açıklama                                         |
| ----------- | ------------------------------------------------ |
| Kullanıcı   | Kullanıcı işlemleri ve kimlik doğrulama          |
| Aidat       | Aidat kayıtlarının görüntülenmesi                |
| Duyuru      | Duyuru oluşturma ve görüntüleme                  |
| Talep       | Arıza ve hizmet talepleri                        |
| Ortak Alan  | Rezervasyona açık ortak alanlar                  |
| Rezervasyon | Rezervasyon oluşturma, görüntüleme ve iptal etme |
| Ortak Gider | Ortak gider kayıtlarının yönetimi                |

---

## HTTP İşlem Türleri

API aşağıdaki temel HTTP yöntemlerini kullanacaktır.

| Yöntem | Amaç                        |
| ------ | --------------------------- |
| GET    | Veri görüntüleme            |
| POST   | Yeni kayıt oluşturma        |
| PUT    | Mevcut kaydı güncelleme     |
| DELETE | Kayıt silme veya iptal etme |

---

## API Tasarım İlkeleri

* Her API isteği belirli bir kaynağa yönelik olmalıdır.
* Yetkilendirme gerektiren işlemler yalnızca yetkili kullanıcılar tarafından gerçekleştirilebilmelidir.
* Hatalı isteklerde kullanıcıya anlaşılır hata mesajları döndürülmelidir.
* API yanıtları tutarlı bir veri yapısına sahip olmalıdır.

---

## Genel Değerlendirme

API tasarımı, BizimSite sisteminin istemci uygulamaları ile güvenli ve düzenli şekilde haberleşmesini sağlamaktadır.

Tanımlanan genel yaklaşım, ilerleyen aşamalarda geliştirilecek API uç noktaları için temel referans niteliğindedir.
