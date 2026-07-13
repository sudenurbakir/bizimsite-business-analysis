# BizimSite - Fonksiyonel Olmayan Gereksinimler

BizimSite sisteminin temel fonksiyonlarını güvenli, kullanılabilir ve tutarlı bir şekilde sunabilmesi için gerekli fonksiyonel olmayan gereksinimler aşağıda tanımlanmıştır.

Fonksiyonel olmayan gereksinimler, sistemin sunduğu işlevlerin hangi kalite ve çalışma koşulları altında gerçekleştirilmesi gerektiğini belirtmektedir.

---

## Değerlendirme Varsayımları

Fonksiyonel olmayan gereksinimler, BizimSite sisteminin ilk sürümü için belirlenen küçük ölçekli site kullanım senaryosu temel alınarak hazırlanmıştır.

Performans gereksinimlerinin değerlendirilmesinde aşağıdaki kullanım koşulları esas alınmıştır:

- 2 blok ve yaklaşık 40 daire
- En fazla 20 eş zamanlı aktif kullanıcı
- İlgili sistem modüllerinde 10.000'e kadar kayıt

Belirlenen değerler, BizimSite projesinin ilk sürümüne ait varsayımsal kullanım koşullarını ifade etmektedir.

---

## 1. Güvenlik

### NFR-01

Sistem, kullanıcı parolalarını düz metin olarak saklamamalıdır.

### NFR-02

Sistem, kullanıcıların yalnızca yetkili oldukları sistem kaynaklarına ve işlemlere erişmesini sağlamalıdır.

### NFR-03

Sistem, kimliği doğrulanmamış kullanıcıların yetkilendirme gerektiren sistem fonksiyonlarına erişmesini engellemelidir.

### NFR-04

Sistem, başarısız giriş denemelerinde kullanıcıya parola veya hesap bilgileri hakkında detaylı sistem bilgisi vermemelidir.

---

## 2. Performans

### NFR-05

Sistem, tanımlanan kullanım koşulları altında temel görüntüleme işlemlerine en fazla 3 saniye içerisinde yanıt vermelidir.

### NFR-06

Sistem, aidat, duyuru, talep, rezervasyon ve ortak gider listelerini 10.000 kayda kadar veri bulunması durumunda en fazla 3 saniye içerisinde görüntülemelidir.

### NFR-07

Sistem, aynı anda en fazla 20 aktif kullanıcının temel görüntüleme ve kayıt işlemlerini gerçekleştirmesini desteklemelidir.

---

## 3. Kullanılabilirlik

### NFR-08

Sistem arayüzü, temel kullanıcı işlemlerinin teknik bilgi gerektirmeden gerçekleştirilebileceği şekilde tasarlanmalıdır.

### NFR-09

Benzer sistem işlemlerinde kullanılan buton, durum ve işlem adlandırmaları tutarlı olmalıdır.

### NFR-10

Sistem, kullanıcı tarafından gerçekleştirilemeyen veya başarısız olan işlemler için anlaşılır hata mesajları göstermelidir.

### NFR-11

Sistem, başarılı şekilde tamamlanan kritik kullanıcı işlemleri sonrasında kullanıcıya işlem sonucuna ilişkin geri bildirim sağlamalıdır.

---

## 4. Veri Gizliliği ve Erişim

### NFR-12

Sistem, kullanıcıların rol ve yetkileri kapsamında erişmesine izin verilen veriler dışındaki özel kullanıcı bilgilerine erişmesini engellemelidir.

### NFR-13

Site sakinlerine ait daire ve finansal bilgiler yalnızca ilgili kullanıcılar ve yetkili yönetim kullanıcıları tarafından görüntülenebilmelidir.

### NFR-14

Sistem, yayımlanmamış finansal kayıtların yetkisiz kullanıcılar tarafından görüntülenmesini engellemelidir.

---

## 5. Uyumluluk ve Erişilebilirlik

### NFR-15

Sistem, güncel masaüstü ve mobil web tarayıcılarında temel fonksiyonlarını kullanılabilir şekilde sunmalıdır.

### NFR-16

Sistem arayüzü, farklı ekran boyutlarında temel işlemlerin gerçekleştirilebilmesini desteklemelidir.

### NFR-17

Metin ve sistem durumları yalnızca görsel renklere bağlı olarak ifade edilmemelidir.

---

## 6. Veri Bütünlüğü

### NFR-18

Sistem, zorunlu alanlar tamamlanmadan ilgili kaydın oluşturulmasını engellemelidir.

### NFR-19

Sistem, kayıt işlemleri sırasında veri bütünlüğünü bozabilecek eksik veya geçersiz verilerin kaydedilmesini engellemelidir.

### NFR-20

Sistem, kullanıcıya başarısız olarak bildirilen bir kayıt işlemini tamamlanmış işlem olarak göstermemelidir.

---

## Fonksiyonel Olmayan Gereksinim Özeti

| Kategori | Gereksinimler |
|---|---|
| Güvenlik | NFR-01 - NFR-04 |
| Performans | NFR-05 - NFR-07 |
| Kullanılabilirlik | NFR-08 - NFR-11 |
| Veri Gizliliği ve Erişim | NFR-12 - NFR-14 |
| Uyumluluk ve Erişilebilirlik | NFR-15 - NFR-17 |
| Veri Bütünlüğü | NFR-18 - NFR-20 |

---

## Genel Değerlendirme

Tanımlanan fonksiyonel olmayan gereksinimler, BizimSite sisteminin temel işlevlerini güvenli, kullanılabilir ve tutarlı bir kullanıcı deneyimi ile sunabilmesi için beklenen kalite koşullarını açıklamaktadır.

Bu gereksinimler, sistem tasarımı, geliştirme ve test süreçlerinde kalite kriterlerinin belirlenmesinde referans olarak kullanılacaktır.
