# BizimSite - Veri Modeli İlişki Kuralları

BizimSite sisteminde yer alan temel veri varlıkları arasındaki ilişkiler ve bu ilişkilerin temel kuralları aşağıda tanımlanmıştır.

Bu kurallar, veri modelindeki kayıtların birbirleriyle tutarlı şekilde ilişkilendirilmesini açıklamaktadır.

---

## 1. Daire ve Aidat İlişkisi

Bir daire birden fazla döneme ait aidat kaydına sahip olabilir.

Her aidat kaydı yalnızca bir daire ile ilişkilendirilmelidir.

Her aidat kaydı ait olduğu dönem ve ödeme durumu bilgisi ile takip edilmelidir.

Aidat ödeme durumu "Ödendi" veya "Ödenmedi" değerlerinden biri olmalıdır.

Aidat kaydı, ilişkili olduğu daire bilgisi bulunmadan oluşturulmamalıdır.

**İlişki:**

`DAIRE 1 - N AIDAT`

---

## 2. Daire ve Kullanıcı İlişkisi

Bir daire birden fazla kullanıcı ile ilişkilendirilebilir.

Bir kullanıcı, sistem kapsamında ilişkili olduğu daire bilgisi üzerinden daireye ait verilere erişebilir.

Kullanıcılar başka dairelere ait özel verilere yetkisiz şekilde erişememelidir.

**İlişki:**

`DAIRE 1 - N KULLANICI`

---

## 3. Kullanıcı ve Duyuru İlişkisi

Bir yetkili kullanıcı birden fazla duyuru oluşturabilir.

Her duyuru, duyuruyu oluşturan kullanıcı ile ilişkilendirilmelidir.

**İlişki:**

`KULLANICI 1 - N DUYURU`

---

## 4. Kullanıcı ve Talep İlişkisi

Bir kullanıcı birden fazla arıza veya hizmet talebi oluşturabilir.

Her talep yalnızca talebi oluşturan bir kullanıcı ile ilişkilendirilmelidir.

Site sakini yalnızca kendi oluşturduğu talepleri takip edebilmelidir.

**İlişki:**

`KULLANICI 1 - N TALEP`

---

## 5. Kullanıcı ve Rezervasyon İlişkisi

Bir kullanıcı birden fazla rezervasyon oluşturabilir.

Her rezervasyon yalnızca rezervasyonu oluşturan bir kullanıcı ile ilişkilendirilmelidir.

Site sakini yalnızca kendi rezervasyon kayıtlarını görüntüleyebilmeli ve iptal edebilmelidir.

**İlişki:**

`KULLANICI 1 - N REZERVASYON`

---

## 6. Ortak Alan ve Rezervasyon İlişkisi

Bir ortak alan için farklı tarih ve saat aralıklarında birden fazla rezervasyon oluşturulabilir.

Her rezervasyon yalnızca bir ortak alan ile ilişkilendirilmelidir.

Aynı ortak alan için çakışan tarih ve saat aralıklarında birden fazla aktif rezervasyon oluşturulmamalıdır.

**İlişki:**

`ORTAK_ALAN 1 - N REZERVASYON`

---

## İlişki Gösterimi Açıklaması

`1 - N` ilişkisi, bir kaydın karşı tarafta birden fazla kayıt ile ilişkilendirilebildiğini ifade eder.

Örneğin bir kullanıcı birden fazla rezervasyon oluşturabilir ancak her rezervasyon yalnızca bir kullanıcı tarafından oluşturulur.

---

## Genel Değerlendirme

Tanımlanan veri modeli ilişki kuralları, BizimSite sistemindeki temel veri varlıklarının birbirleriyle nasıl ilişkilendirileceğini açıklamaktadır.

Bu kurallar, veritabanı ilişkilerinin oluşturulması ve veri bütünlüğünün korunması süreçlerinde referans olarak kullanılacaktır.
