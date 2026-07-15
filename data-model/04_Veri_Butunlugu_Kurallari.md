# BizimSite - Veri Bütünlüğü Kuralları

BizimSite sisteminde tutulan verilerin ilişkisel bütünlüğünü ve tutarlılığını korumak amacıyla temel veri bütünlüğü kuralları tanımlanmıştır.

Bu kurallar, sistem içerisindeki ilişkili kayıtların geçerli ve tutarlı şekilde yönetilmesini amaçlamaktadır.

---

## Kullanıcı ve Daire Bütünlüğü

Kullanıcı ile ilişkilendirilen daire kaydı sistemde mevcut olmalıdır.

Geçersiz veya sistemde bulunmayan bir daire kaydı ile kullanıcı ilişkisi oluşturulmamalıdır.

---

## Daire ve Aidat Bütünlüğü

Her aidat kaydı mevcut bir daire ile ilişkilendirilmelidir.

Bir daire birden fazla döneme ait aidat kaydına sahip olabilir.

Her aidat kaydı ait olduğu dönem ve ödeme durumu bilgisi ile takip edilmelidir.

Aidat ödeme durumu "Ödendi" veya "Ödenmedi" değerlerinden biri olmalıdır.

Aynı daire ve aynı dönem için birden fazla aidat kaydı oluşturulmamalıdır.

---

## Kullanıcı ve Duyuru Bütünlüğü

Her duyuru, sistemde kayıtlı ve yetkili bir kullanıcı tarafından oluşturulmalıdır.

Duyuruyu oluşturan kullanıcı bilgisi geçerli bir kullanıcı kaydı ile ilişkilendirilmelidir.

---

## Kullanıcı ve Talep Bütünlüğü

Her arıza veya hizmet talebi, talebi oluşturan kullanıcı ile ilişkilendirilmelidir.

Sistemde bulunmayan bir kullanıcı adına talep kaydı oluşturulmamalıdır.

---

## Kullanıcı ve Rezervasyon Bütünlüğü

Her rezervasyon, rezervasyonu oluşturan geçerli bir kullanıcı ile ilişkilendirilmelidir.

Rezervasyon kaydındaki kullanıcı ilişkisi korunmalıdır.

Site sakini yalnızca kendi rezervasyon kayıtlarını görüntüleyebilmeli ve iptal edebilmelidir.

---

## Ortak Alan ve Rezervasyon Bütünlüğü

Her rezervasyon mevcut bir ortak alan ile ilişkilendirilmelidir.

Sistemde bulunmayan bir ortak alan için rezervasyon oluşturulmamalıdır.

Aynı ortak alan için çakışan tarih ve saat aralıklarında birden fazla aktif rezervasyon oluşturulmamalıdır.

Aktif rezervasyonlarla ilişkili ortak alan kayıtları kaldırılmadan önce mevcut rezervasyon ilişkileri kontrol edilmelidir.

---

## Kayıt İlişkilerinin Korunması

Başka kayıtlar ile ilişkili olan bir kayıt kaldırılmadan önce mevcut veri ilişkileri kontrol edilmelidir.

Örneğin aidat kayıtları bulunan bir daire veya rezervasyon kayıtları bulunan bir ortak alan kaldırılırken ilişkili kayıtların bağlantısız hale gelmesi önlenmelidir.

Sistem içerisindeki veri ilişkileri ve kayıt tutarlılığı korunmalıdır.

---

## Genel Değerlendirme

Veri bütünlüğü kuralları, BizimSite sistemindeki ilişkili kayıtların geçerli ve tutarlı şekilde yönetilmesini sağlamaktadır.

Bu kurallar, veritabanı ilişkilerinin ve veri koruma mekanizmalarının tasarlanmasında referans olarak kullanılacaktır.
