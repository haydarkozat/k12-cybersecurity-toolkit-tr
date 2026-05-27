# Metodoloji

> Bu doküman proje boyunca doldurulacaktır. Hafta 1 sonunda ilk versiyonu yayınlanacak.

## 1. Yaklaşım

Bu çalışma, bir gri-kutu (gray-box) güvenlik değerlendirmesi yaklaşımı benimser:
- **Beyaz-kutu**: Yapılandırma dosyalarına ve sistem detaylarına okuma erişimi var
- **Kara-kutu**: Saldırgan perspektifinden bilinmeyen sistem
- **Gri-kutu** (bu çalışma): Sınırlı yetkilerle sistem incelemesi + harici görünüm

## 2. Kullanılan Çerçeveler

### 2.1 NIST Cybersecurity Framework 2.0
Bkz. `01-nist-csf-2-uyarlama.md`

### 2.2 CIS Controls v8 IG1
Küçük ve orta ölçekli kuruluşlar için temel kontrol seti. K-12 okullarına en uygun olgunluk grubu olan IG1 (Implementation Group 1) seçilmiştir.

### 2.3 KVKK Uyumluluk
Bkz. `02-kvkk-okullar-icin.md`

### 2.4 MEB Bilişim Güvenliği Rehberi
Bkz. `03-meb-rehberi-eslestirme.md`

## 3. Veri Toplama Yöntemleri

| Yöntem | Faaliyet | Kapsam |
|---|---|---|
| Doküman incelemesi | Mevcut config, log, politika | Hafta 2 |
| Yapılandırma incelemesi | Read-only switch/router config | Hafta 3 |
| Aktif tarama | Nmap envanter taraması | Hafta 3 |
| Zafiyet taraması | OpenVAS / Nessus Essentials | Hafta 3 |
| Pasif gözlem | Wireshark pasif yakalama | Hafta 3 |
| Mülakat/anket | Personel farkındalık | Hafta 2-3 |

## 4. Risk Değerlendirme Modeli

(Hafta 1'de detaylandırılacak)

CVSS v3.1 + kuruma özgü etki çarpanları:
- Eğitim faaliyetlerine etki
- Öğrenci verisi etkilenmesi (KVKK)
- Tarihsel olasılık
- Tespit ve müdahale gecikmesi

## 5. Olgunluk Skorlama

NIST CSF 2.0 Tier modeli:
- Tier 1: Partial (Kısmi)
- Tier 2: Risk Informed (Risk Bilgili)
- Tier 3: Repeatable (Tekrarlanabilir)
- Tier 4: Adaptive (Uyarlanabilir)

Her fonksiyon (Govern, Identify, Protect, Detect, Respond, Recover) için ayrı skorlama yapılır.

## 6. Sınırlamalar

- Tek bir okul üzerinden yapılan değerlendirme, tüm K-12 okullarına genelleştirilemez
- Aktif tarama eğitim faaliyetlerini etkilememek için sınırlı tutulmuştur
- Penetrasyon testi yapılmamıştır (kapsamı bilinçli olarak dışında bırakılmıştır)
- Çalışma süresi 5 hafta ile sınırlıdır
