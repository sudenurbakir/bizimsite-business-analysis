# BizimSite - Ortak Alan Rezervasyonu Use Case Analizi

BizimSite ortak alan rezervasyonu süreci kapsamında kullanıcılar ile sistem arasındaki temel etkileşimler aşağıda use case olarak tanımlanmıştır.

---

## UC-15 - Rezervasyona Açık Ortak Alanları Görüntüleme

### Aktör

Site Sakini

### Amaç

Site sakininin rezervasyon oluşturabileceği ortak alanları görüntülemesini sağlamak.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.

### Tetikleyici

Site sakininin rezervasyona açık ortak alanları görüntülemek istemesi.

### Ana Akış

1. Site sakini ortak alan rezervasyonu ekranını açar.
2. Sistem rezervasyona açık ortak alanları belirler.
3. Sistem ilgili ortak alanları kullanıcıya görüntüler.
4. Site sakini görüntülemek istediği ortak alanı seçer.
5. Sistem seçilen ortak alanın bilgilerini görüntüler.

### Alternatif Akışlar

#### A1 - Rezervasyona Açık Ortak Alan Bulunmaması

1. Sistem rezervasyona açık ortak alan bulunmadığını tespit eder.
2. Sistem kullanıcıya rezervasyona açık ortak alan bulunmadığını bildirir.

### Son Koşullar

- Site sakini rezervasyona açık ortak alanları görüntüler.

### İlgili Kullanıcı Hikayesi

- US-15

---

## UC-16 - Ortak Alan Rezervasyonu Oluşturma

### Aktör

Site Sakini

### Amaç

Rezervasyona açık bir ortak alan için tarih ve saat aralığı belirleyerek rezervasyon oluşturulmasını sağlamak.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.
- İlgili ortak alan rezervasyona açık olmalıdır.

### Tetikleyici

Site sakininin bir ortak alan için rezervasyon oluşturmak istemesi.

### Ana Akış

1. Site sakini rezervasyona açık ortak alanı seçer.
2. Sistem rezervasyon formunu görüntüler.
3. Site sakini tarih ve saat aralığını girer.
4. Site sakini rezervasyon işlemini başlatır.
5. Sistem girilen bilgileri doğrular.
6. Sistem seçilen zaman aralığındaki aktif rezervasyonları kontrol eder.
7. Sistem rezervasyonu kullanıcı ile ilişkilendirir.
8. Sistem rezervasyon kaydını oluşturur.
9. Sistem kullanıcıya işlemin başarılı olduğunu bildirir.

### Alternatif Akışlar

#### A1 - Zorunlu Alanların Eksik Olması

1. Sistem zorunlu alanların eksik olduğunu tespit eder.
2. Sistem rezervasyon kaydını oluşturmaz.
3. Sistem kullanıcıya eksik alanlara ilişkin hata mesajı gösterir.

#### A2 - Geçmiş Tarihli Zaman Aralığı

1. Sistem seçilen zaman aralığının geçmiş tarihli olduğunu tespit eder.
2. Sistem rezervasyon kaydını oluşturmaz.
3. Sistem kullanıcıya hata mesajı gösterir.

#### A3 - Çakışan Rezervasyon Bulunması

1. Sistem aynı ortak alan için seçilen zaman aralığıyla çakışan aktif bir rezervasyon bulunduğunu tespit eder.
2. Sistem rezervasyon kaydını oluşturmaz.
3. Sistem kullanıcıya seçilen zaman aralığının uygun olmadığını bildirir.

### Son Koşullar

- Rezervasyon, site sakini ve ilgili ortak alan ile ilişkilendirilmiş şekilde sistemde kayıt altına alınır.

### İlgili Kullanıcı Hikayeleri

- US-16
- US-17

---

## UC-17 - Kendi Rezervasyonlarını Görüntüleme

### Aktör

Site Sakini

### Amaç

Site sakininin oluşturduğu ortak alan rezervasyonlarını takip etmesini sağlamak.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.

### Tetikleyici

Site sakininin kendi rezervasyonlarını görüntülemek istemesi.

### Ana Akış

1. Site sakini rezervasyon ekranını açar.
2. Sistem kullanıcı tarafından oluşturulan rezervasyonları belirler.
3. Sistem ilgili rezervasyon kayıtlarını getirir.
4. Sistem ortak alan, tarih ve saat bilgilerini kullanıcıya görüntüler.

### Alternatif Akışlar

#### A1 - Rezervasyon Kaydı Bulunmaması

1. Sistem kullanıcı tarafından oluşturulmuş rezervasyon kaydı bulunmadığını tespit eder.
2. Sistem kullanıcıya görüntülenecek rezervasyon bulunmadığını bildirir.

### Son Koşullar

- Site sakini kendi rezervasyon kayıtlarını görüntüler.

### İlgili Kullanıcı Hikayesi

- US-18

## US-19 - Rezervasyon İptal Etme

### Kullanıcı Hikayesi

Bir site sakini olarak, oluşturduğum ve henüz gerçekleşmemiş bir rezervasyonu iptal etmek istiyorum; böylece kullanmayacağım ortak alan rezervasyonunu kaldırabilirim.

### Kabul Kriterleri

- Site sakini yalnızca kendi oluşturduğu rezervasyonları iptal edebilmelidir.
- Geçmiş rezervasyonlar iptal edilememelidir.
- Başka kullanıcılar tarafından oluşturulan rezervasyonlar iptal edilememelidir.
- Başarılı iptal işlemi sonrasında kullanıcıya işlem sonucu bildirilmelidir.

## Genel Değerlendirme

Ortak alan rezervasyonu use case analizi, site sakinlerinin rezervasyona açık ortak alanları görüntülemesi, uygun tarih ve saat aralıkları için rezervasyon oluşturması ve kendi rezervasyon kayıtlarını takip etmesi süreçlerini açıklamaktadır.

Tanımlanan ana ve alternatif akışlar, sistem davranışlarının detaylandırılması ve sonraki tasarım çalışmalarında referans olarak kullanılacaktır.
