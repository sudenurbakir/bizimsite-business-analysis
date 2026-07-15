# BizimSite - Kullanıcı Yetkilendirme Use Case Analizi

BizimSite kullanıcı yetkilendirme süreci kapsamında kullanıcıların sistem içerisindeki işlem ve veri erişimlerinin sahip oldukları roller doğrultusunda kontrol edilmesine yönelik temel etkileşimler aşağıda use case olarak tanımlanmıştır.

---

## UC-23 - Rol Kapsamındaki İşlemlere Erişim

### Aktör

Sistem Kullanıcısı

### Amaç

Kullanıcının sahip olduğu rol kapsamında izin verilen sistem işlemlerine erişmesini sağlamak.

### Ön Koşullar

- Kullanıcı sisteme giriş yapmış olmalıdır.
- Kullanıcıya sistemde bir rol atanmış olmalıdır.

### Tetikleyici

Kullanıcının yetkilendirme gerektiren bir sistem işlemine erişmek istemesi.

### Ana Akış

1. Kullanıcı sistemde bir işlem başlatır.
2. Sistem kullanıcının kimliğini doğrular.
3. Sistem kullanıcının rol bilgilerini belirler.
4. Sistem ilgili işlem için gerekli yetkileri kontrol eder.
5. Sistem kullanıcının işlem için yetkili olduğunu tespit eder.
6. Sistem kullanıcının ilgili işleme erişmesine izin verir.

### Alternatif Akışlar

#### A1 - Yetkisiz İşlem

1. Sistem kullanıcının ilgili işlem için gerekli yetkiye sahip olmadığını tespit eder.
2. Sistem işleme erişimi engeller.
3. Sistem kullanıcıya işlemi gerçekleştirme yetkisi bulunmadığını bildirir.

#### A2 - Kimliği Doğrulanmamış Kullanıcı

1. Sistem kullanıcının kimliğinin doğrulanmadığını tespit eder.
2. Sistem yetkilendirme gerektiren işleme erişimi engeller.
3. Sistem kullanıcıdan sisteme giriş yapmasını ister.

### Son Koşullar

- Yetkili kullanıcı ilgili sistem işlemine erişir.
- Yetkisiz erişim girişimleri engellenir.

### İlgili Kullanıcı Hikayesi

- US-24

---

## UC-24 - Yönetim İşlemlerini Yetkisiz Erişimden Koruma

### Aktör

Site Sakini

### Amaç

Yönetim yetkisi gerektiren işlemlerin yetkisiz kullanıcılar tarafından gerçekleştirilmesini engellemek.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.
- Kullanıcının yönetim yetkisi bulunmamalıdır.

### Tetikleyici

Site sakininin yönetim yetkisi gerektiren bir işlemi gerçekleştirmeye çalışması.

### Ana Akış

1. Site sakini yönetim yetkisi gerektiren bir işlemi başlatmaya çalışır.
2. Sistem kullanıcının rol ve yetki bilgilerini kontrol eder.
3. Sistem kullanıcının yönetim yetkisine sahip olmadığını tespit eder.
4. Sistem işlemin gerçekleştirilmesini engeller.
5. Sistem kullanıcıya ilgili işlem için yetkisi bulunmadığını bildirir.

### Alternatif Akışlar

#### A1 - Kullanıcının Yetkili Olması

1. Sistem kullanıcının ilgili işlem için gerekli yetkiye sahip olduğunu tespit eder.
2. Sistem kullanıcının ilgili işleme devam etmesine izin verir.

### Son Koşullar

- Yetkisiz kullanıcı yönetim işlemini gerçekleştiremez.
- Yönetim işlemlerine erişim kullanıcı yetkileri doğrultusunda kontrol edilir.

### İlgili Kullanıcı Hikayesi

- US-25

---

## UC-25 - Özel Kullanıcı Bilgilerine Erişimi Kontrol Etme

### Aktör

Site Sakini

### Amaç

Özel kullanıcı bilgilerinin yalnızca ilgili kullanıcılar ve yetkili kullanıcılar tarafından görüntülenmesini sağlamak.

### Ön Koşullar

- Site sakini sisteme giriş yapmış olmalıdır.

### Tetikleyici

Site sakininin özel kullanıcı bilgisi içeren bir sistem kaynağına erişmek istemesi.

### Ana Akış

1. Site sakini özel kullanıcı bilgisi içeren bir kaynağa erişmek ister.
2. Sistem kullanıcının kimlik ve rol bilgilerini kontrol eder.
3. Sistem kullanıcının ilgili veriye erişim yetkisini değerlendirir.
4. Sistem kullanıcının veriye erişim yetkisi bulunduğunu tespit eder.
5. Sistem ilgili bilgileri kullanıcıya görüntüler.

### Alternatif Akışlar

#### A1 - Başka Kullanıcıya Ait Özel Bilgi

1. Sistem ilgili bilgilerin başka bir site sakinine ait olduğunu tespit eder.
2. Sistem kullanıcının ilgili verilere erişim yetkisi bulunmadığını belirler.
3. Sistem verilere erişimi engeller.

#### A2 - Yetkisiz Kullanıcı

1. Sistem kullanıcının ilgili özel bilgileri görüntüleme yetkisine sahip olmadığını tespit eder.
2. Sistem verilere erişimi engeller.
3. Sistem kullanıcıya erişim yetkisi bulunmadığını bildirir.

### Son Koşullar

- Özel kullanıcı bilgileri yalnızca erişim yetkisi bulunan kullanıcılar tarafından görüntülenir.
- Yetkisiz veri erişimleri engellenir.

### İlgili Kullanıcı Hikayesi

- US-26

---

## Genel Değerlendirme

Kullanıcı yetkilendirme use case analizi, sistem kullanıcılarının sahip oldukları roller kapsamında işlemlere erişmesi, yönetim işlemlerinin yetkisiz kullanıcılardan korunması ve özel kullanıcı bilgilerinin erişim yetkileri doğrultusunda görüntülenmesi süreçlerini açıklamaktadır.

Tanımlanan ana ve alternatif akışlar, sistem davranışlarının detaylandırılması ve sonraki tasarım çalışmalarında referans olarak kullanılacaktır.
