# BizimSite - Sistem Mimarisi

BizimSite sisteminin temel bileşenleri ve bu bileşenler arasındaki genel iletişim yapısı aşağıda tanımlanmıştır.

Sistem mimarisi, kullanıcı işlemlerinin arayüz, uygulama ve veri katmanları üzerinden kontrollü şekilde yürütülmesini temel almaktadır.

---

## Mimari Yaklaşım

BizimSite sistemi katmanlı mimari yaklaşımı temel alınarak tasarlanacaktır.

Sistem temel olarak aşağıdaki katmanlardan oluşmaktadır:

* Kullanıcı Arayüzü Katmanı
* Uygulama Katmanı
* Veri Katmanı

---

## Kullanıcı Arayüzü Katmanı

Kullanıcıların BizimSite sistemi ile etkileşim kurduğu katmandır.

Site sakinleri ve yetkili kullanıcılar, sahip oldukları rol kapsamında sistem fonksiyonlarına kullanıcı arayüzü üzerinden erişir.

Kullanıcı arayüzü aşağıdaki temel işlemlerin gerçekleştirilmesini sağlar:

* Aidat bilgilerinin görüntülenmesi
* Duyuruların görüntülenmesi ve yönetilmesi
* Arıza ve hizmet taleplerinin oluşturulması ve takip edilmesi
* Ortak alan rezervasyonlarının oluşturulması, görüntülenmesi ve iptal edilmesi
* Ortak gider bilgilerinin görüntülenmesi ve yönetilmesi

---

## Uygulama Katmanı

Kullanıcı arayüzünden gelen işlemlerin sistem kuralları doğrultusunda değerlendirildiği katmandır.

Bu katman iş kurallarının, yetkilendirme kontrollerinin ve veri doğrulama işlemlerinin uygulanmasından sorumludur.

Örneğin sistem, rezervasyon oluşturma işlemi sırasında ortak alanın rezervasyona açık olup olmadığını ve seçilen zaman aralığında çakışan aktif bir rezervasyon bulunup bulunmadığını kontrol eder.

---

## Veri Katmanı

Sistem içerisinde kullanılan verilerin saklanması ve yönetilmesinden sorumlu katmandır.

Kullanıcı, daire, aidat, duyuru, talep, ortak alan, rezervasyon ve ortak gider kayıtları veri katmanında yönetilir.

Veri ilişkileri ve veri bütünlüğü kuralları bu katmanda dikkate alınmalıdır.

---

## Katmanlar Arası İletişim

Kullanıcı işlemleri kullanıcı arayüzü üzerinden başlatılır.

İşlem uygulama katmanına iletilir ve ilgili iş kuralları ile doğrulama kontrolleri uygulanır.

Geçerli işlemler veri katmanına iletilerek gerekli veri işlemleri gerçekleştirilir.

İşlem sonucu kullanıcı arayüzü üzerinden kullanıcıya bildirilir.

---

## Genel Değerlendirme

BizimSite sistem mimarisi, kullanıcı arayüzü, uygulama ve veri katmanlarının sorumluluklarının ayrılmasını temel almaktadır.

Katmanlı mimari yaklaşımı, sistem bileşenlerinin daha düzenli, yönetilebilir ve geliştirilebilir şekilde tasarlanmasına katkı sağlamaktadır.
