# BizimSite - Varlık İlişki Diyagramı

BizimSite sisteminde yer alan temel veri varlıkları ve bu varlıklar arasındaki ilişkiler aşağıdaki varlık ilişki diyagramında gösterilmiştir.

---

## Varlık İlişki Diyagramı

```mermaid
erDiagram

    KULLANICI {
        int kullanici_id PK
        string ad
        string soyad
        string eposta
        string parola
        string rol
    }

    DAIRE {
        int daire_id PK
        string blok
        string daire_no
    }

    AIDAT {
        int aidat_id PK
        int daire_id FK
        string donem
        decimal tutar
        string odeme_durumu
    }

    DUYURU {
        int duyuru_id PK
        int olusturan_kullanici_id FK
        string baslik
        string icerik
        string durum
        datetime yayimlanma_tarihi
    }

    TALEP {
        int talep_id PK
        int kullanici_id FK
        string talep_turu
        string aciklama
        string durum
        datetime olusturma_tarihi
    }

    ORTAK_ALAN {
        int ortak_alan_id PK
        string ad
        boolean rezervasyona_acik
    }

    REZERVASYON {
        int rezervasyon_id PK
        int kullanici_id FK
        int ortak_alan_id FK
        datetime baslangic_tarihi
        datetime bitis_tarihi
        string durum
    }

    ORTAK_GIDER {
        int ortak_gider_id PK
        string gider_turu
        string donem
        decimal tutar
        string durum
    }

    DAIRE ||--o{ AIDAT : "aittir"
    DAIRE ||--o{ KULLANICI : "iliskilidir"

    KULLANICI ||--o{ DUYURU : "olusturur"
    KULLANICI ||--o{ TALEP : "olusturur"
    KULLANICI ||--o{ REZERVASYON : "olusturur"

    ORTAK_ALAN ||--o{ REZERVASYON : "icin kullanilir"
```

---

## Temel Varlıklar

### Kullanıcı

Sisteme erişen site sakini ve yetkili kullanıcıların temel bilgilerini temsil eder.

### Daire

Site içerisinde bulunan daire kayıtlarını temsil eder.

### Aidat

Dairelere ait dönemsel aidat kayıtlarını ve ödeme durumlarını temsil eder.

### Duyuru

Site yönetimi tarafından oluşturulan taslak veya yayımlanmış duyuru kayıtlarını temsil eder.

### Talep

Site sakinleri tarafından oluşturulan arıza ve hizmet taleplerini temsil eder.

### Ortak Alan

Rezervasyon işlemine konu olabilecek ortak kullanım alanlarını temsil eder.

### Rezervasyon

Site sakinlerinin ortak alanlar için oluşturduğu rezervasyon kayıtlarını temsil eder.

### Ortak Gider

Site veya apartmana ait ortak kullanım giderlerini temsil eder.

---

## İlişki Açıklamaları

Bir daire birden fazla aidat kaydına sahip olabilir. Her aidat kaydı yalnızca bir daire ile ilişkilidir.

Bir daire birden fazla kullanıcı ile ilişkilendirilebilir. Her kullanıcı bir daire ile ilişkilidir.

Bir kullanıcı birden fazla duyuru, talep veya rezervasyon kaydı oluşturabilir.

Bir ortak alan birden fazla rezervasyon kaydına sahip olabilir. Her rezervasyon yalnızca bir ortak alan ile ilişkilidir.

---

## Genel Değerlendirme

Varlık ilişki diyagramı, BizimSite sisteminde yönetilecek temel veri varlıklarını ve bu varlıklar arasındaki ilişkileri göstermektedir.

Diyagram, veritabanı tasarımının detaylandırılması ve sistem veri modelinin oluşturulması süreçlerinde referans olarak kullanılacaktır.
