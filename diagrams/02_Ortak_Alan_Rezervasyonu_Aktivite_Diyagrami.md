# BizimSite - Ortak Alan Rezervasyonu Activity Diagramı

BizimSite ortak alan rezervasyonu sürecinde site sakini ile sistem arasındaki temel işlem akışı aşağıdaki activity diagramında gösterilmiştir.

---

## Activity Diagramı

```mermaid
flowchart TD

    A([Başlangıç]) --> B[Ortak alanları görüntüle]
    B --> C[Ortak alan seç]
    C --> D[Tarih ve saat aralığı belirle]
    D --> E[Rezervasyon işlemini başlat]

    E --> F{Bilgiler geçerli mi?}

    F -- Hayır --> G[Hata mesajı göster]
    G --> D

    F -- Evet --> H{Zaman aralığı geçmiş mi?}

    H -- Evet --> I[Rezervasyon oluşturma işlemini engelle]
    I --> D

    H -- Hayır --> J{Çakışan aktif rezervasyon var mı?}

    J -- Evet --> K[Zaman aralığının uygun olmadığını bildir]
    K --> D

    J -- Hayır --> L[Rezervasyonu kullanıcı ile ilişkilendir]
    L --> M[Rezervasyon kaydını oluştur]
    M --> N[Başarılı işlem bildirimi göster]
    N --> O([Bitiş])
```

---

## Süreç Açıklaması

Site sakini rezervasyona açık bir ortak alan seçerek tarih ve saat aralığını belirler.

Sistem, rezervasyon bilgilerini doğrular ve seçilen zaman aralığının geçmiş tarihli olup olmadığını kontrol eder. Ardından aynı ortak alan için çakışan aktif bir rezervasyon bulunup bulunmadığını değerlendirir.

Tüm kontrollerin başarılı olması durumunda rezervasyon kullanıcı ile ilişkilendirilerek sistemde kayıt altına alınır.

---

## İlgili Use Case'ler

- UC-15 - Rezervasyona Açık Ortak Alanları Görüntüleme
- UC-16 - Ortak Alan Rezervasyonu Oluşturma

---

## Genel Değerlendirme

Ortak alan rezervasyonu activity diagramı, rezervasyon oluşturma sürecindeki temel karar noktalarını ve sistem kontrollerini görsel olarak açıklamaktadır.

Diyagram, rezervasyon sürecinin sistem tasarımı ve geliştirme aşamalarında değerlendirilmesinde referans olarak kullanılacaktır.
