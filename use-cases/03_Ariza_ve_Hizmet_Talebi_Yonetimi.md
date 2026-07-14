# BizimSite - Arıza ve Hizmet Talebi Yönetimi Use Case Analizi

BizimSite arıza ve hizmet talebi yönetimi süreci kapsamında kullanıcılar ile sistem arasındaki temel etkileşimler aşağıda use case olarak tanımlanmıştır.

---

## UC-09 - Arıza veya Hizmet Talebi Oluşturma

### Aktör

Site Sakini

### Amaç

Site sakininin yaşadığı arıza veya hizmet ihtiyacını site yönetimine iletmesini sağlamak.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.
- Kullanıcının talep oluşturma yetkisi bulunmalıdır.

### Tetikleyici

Site sakininin yeni arıza veya hizmet talebi oluşturmak istemesi.

### Ana Akış

1. Site sakini talep yönetimi ekranını açar.
2. Yeni talep oluşturma işlemini başlatır.
3. Sistem talep formunu görüntüler.
4. Site sakini talep açıklamasını girer.
5. Site sakini kayıt işlemini başlatır.
6. Sistem girilen bilgileri doğrular.
7. Sistem talebi kullanıcı ile ilişkilendirir.
8. Sistem talebi "Yeni" durumuyla kaydeder.
9. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Zorunlu Alanların Eksik Olması

1. Sistem zorunlu alanların eksik olduğunu tespit eder.
2. Sistem talebi oluşturmaz.
3. Sistem kullanıcıya eksik alanlara ilişkin hata mesajı gösterir.

### Son Koşullar

- Talep, site sakini ile ilişkilendirilmiş ve "Yeni" durumunda sistemde kayıt altına alınır.

### İlgili Kullanıcı Hikayesi

- US-09

---

## UC-10 - Talebi Teknik Ekibe Yönlendirme

### Aktör

Site Yöneticisi

### Amaç

Oluşturulan talebin ilgili teknik ekip personeline yönlendirilmesini sağlamak.

### Ön Koşullar

- Site yöneticisi sisteme giriş yapmış olmalıdır.
- İlgili talep sistemde bulunmalıdır.
- Teknik ekip personeli sistemde tanımlı olmalıdır.

### Tetikleyici

Site yöneticisinin bir talebi teknik ekip personeline yönlendirmek istemesi.

### Ana Akış

1. Site yöneticisi talep yönetimi ekranını açar.
2. Sistem mevcut talepleri görüntüler.
3. Site yöneticisi yönlendirilecek talebi seçer.
4. Sistem talep bilgilerini görüntüler.
5. Site yöneticisi ilgili teknik ekip personelini seçer.
6. Site yöneticisi yönlendirme işlemini başlatır.
7. Sistem talebi seçilen teknik ekip personeli ile ilişkilendirir.
8. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Teknik Ekip Personeli Seçilmemesi

1. Sistem teknik ekip personeli seçilmediğini tespit eder.
2. Sistem yönlendirme işlemini gerçekleştirmez.
3. Sistem kullanıcıya hata mesajı gösterir.

### Son Koşullar

- Talep ilgili teknik ekip personeline atanmış olarak sistemde saklanır.

### İlgili Kullanıcı Hikayesi

- US-10

---

## UC-11 - Atanan Talepleri Görüntüleme

### Aktör

Teknik Ekip Personeli

### Amaç

Teknik ekip personelinin kendisine atanan talepleri görüntülemesini sağlamak.

### Ön Koşullar

- Teknik ekip personeli sisteme giriş yapmış olmalıdır.

### Tetikleyici

Teknik ekip personelinin kendisine atanan talepleri görüntülemek istemesi.

### Ana Akış

1. Teknik ekip personeli talep ekranını açar.
2. Sistem kullanıcı ile ilişkilendirilmiş talepleri belirler.
3. Sistem yalnızca ilgili personele atanmış talepleri getirir.
4. Sistem talep açıklaması ve mevcut durum bilgilerini görüntüler.

### Alternatif Akışlar

#### A1 - Atanmış Talep Bulunmaması

1. Sistem kullanıcıya atanmış talep bulunmadığını tespit eder.
2. Sistem kullanıcıya görüntülenecek talep bulunmadığını bildirir.

### Son Koşullar

- Teknik ekip personeli kendisine atanmış mevcut talepleri görüntüler.

### İlgili Kullanıcı Hikayesi

- US-11

---

## UC-12 - Talep Durumunu Güncelleme

### Aktör

Teknik Ekip Personeli

### Amaç

Atanmış bir talebin mevcut işlem durumunun güncellenmesini sağlamak.

### Ön Koşullar

- Teknik ekip personeli sisteme giriş yapmış olmalıdır.
- İlgili talep teknik ekip personeline atanmış olmalıdır.

### Tetikleyici

Teknik ekip personelinin talep durumunu güncellemek istemesi.

### Ana Akış

1. Teknik ekip personeli kendisine atanmış talepleri görüntüler.
2. Güncellenecek talebi seçer.
3. Sistem talebin mevcut bilgilerini görüntüler.
4. Teknik ekip personeli talep durumunu seçer.
5. Teknik ekip personeli güncelleme işlemini başlatır.
6. Sistem seçilen durum bilgisini doğrular.
7. Sistem talep durumunu günceller.
8. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Geçersiz Talep Durumu

1. Sistem seçilen durumun tanımlı değerlerden biri olmadığını tespit eder.
2. Sistem güncelleme işlemini gerçekleştirmez.
3. Sistem kullanıcıya hata mesajı gösterir.

#### A2 - Kullanıcıya Atanmamış Talep

1. Sistem talebin ilgili teknik ekip personeline atanmadığını tespit eder.
2. Sistem güncelleme işlemini engeller.

### Son Koşullar

- Talebin güncel durum bilgisi sistemde saklanır.

### İlgili Kullanıcı Hikayesi

- US-12

---

## UC-13 - Kendi Taleplerinin Durumunu Görüntüleme

### Aktör

Site Sakini

### Amaç

Site sakininin oluşturduğu taleplerin mevcut durumunu takip etmesini sağlamak.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.

### Tetikleyici

Site sakininin oluşturduğu talepleri görüntülemek istemesi.

### Ana Akış

1. Site sakini talep ekranını açar.
2. Sistem kullanıcı tarafından oluşturulan talepleri belirler.
3. Sistem ilgili talepleri getirir.
4. Sistem taleplerin güncel durum bilgilerini görüntüler.

### Alternatif Akışlar

#### A1 - Talep Bulunmaması

1. Sistem kullanıcı tarafından oluşturulmuş talep bulunmadığını tespit eder.
2. Sistem kullanıcıya görüntülenecek talep bulunmadığını bildirir.

### Son Koşullar

- Site sakini kendi taleplerinin mevcut durumlarını görüntüler.

### İlgili Kullanıcı Hikayesi

- US-13

---

## UC-14 - Geçmiş Talepleri Görüntüleme

### Aktör

Site Yöneticisi

### Amaç

Geçmiş arıza ve hizmet taleplerinin takip edilmesini sağlamak.

### Ön Koşullar

- Site yöneticisi sisteme giriş yapmış olmalıdır.
- Kullanıcının talep kayıtlarını görüntüleme yetkisi bulunmalıdır.

### Tetikleyici

Site yöneticisinin geçmiş talepleri görüntülemek istemesi.

### Ana Akış

1. Site yöneticisi talep yönetimi ekranını açar.
2. Sistem geçmiş talep kayıtlarını getirir.
3. Sistem talepleri mevcut durum bilgileri ile görüntüler.
4. Site yöneticisi görüntülemek istediği talebi seçer.
5. Sistem seçilen talebin bilgilerini görüntüler.

### Alternatif Akışlar

#### A1 - Geçmiş Talep Bulunmaması

1. Sistem geçmiş talep kaydı bulunmadığını tespit eder.
2. Sistem kullanıcıya görüntülenecek talep bulunmadığını bildirir.

### Son Koşullar

- Site yöneticisi geçmiş talep kayıtlarını görüntüler.

### İlgili Kullanıcı Hikayesi

- US-14

---

## Genel Değerlendirme

Arıza ve hizmet talebi yönetimi use case analizi, site sakinlerinin talep oluşturması ve taleplerini takip etmesi, site yöneticisinin talepleri teknik ekibe yönlendirmesi ve teknik ekip personelinin kendisine atanan talepleri yönetmesi süreçlerini açıklamaktadır.

Tanımlanan ana ve alternatif akışlar, sistem davranışlarının detaylandırılması ve sonraki tasarım çalışmalarında referans olarak kullanılacaktır.
