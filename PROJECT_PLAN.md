# Proje Planı ve Teslim Edilecekler Matrisi

**Proje:** Hüyük Ortaokulu Bilgi Güvenliği Değerlendirmesi
**Yürütücü:** Haydar KOZAT (Okul Bilişim Sorumlusu)
**Süre:** 13.03.2026 – 19.04.2026 (5 hafta)
**Çerçeve:** NIST CSF 2.0 + KVKK + CIS Controls v8 IG1

---

## 5 Haftalık Takvim

| Hafta | Tarih | Faz | Ana İş |
|---|---|---|---|
| **1** | 13–20 Mart | Hazırlık | Yetki belgesinin imzalanması, metodoloji çalışması, çerçeve uyarlama |
| **2** | 21–27 Mart | Veri toplama I | Doküman incelemesi, donanım envanteri, network diyagramı çıkarma |
| **3** | 28 Mart – 4 Nisan | Veri toplama II | Yapılandırma incelemesi, mesai dışı aktif tarama, KVKK uyum kontrolü |
| **4** | 5–12 Nisan | Değerlendirme | NIST CSF olgunluk skorlaması, risk dereceleme, bulguların önceliklendirilmesi |
| **5** | 13–19 Nisan | Raporlama | Detaylı rapor, yönetici özeti sunumu, anonimleştirilmiş public içerik |

---

## Teslim Edilecekler Matrisi

### 🌐 Halka açık (GitHub'a gidecek)

| # | Teslim Edilecek | Format | Hafta | Açıklama |
|---|---|---|---|---|
| P1 | README.md | Markdown | 1 | Proje girişi (hazır) |
| P2 | PROJECT_PLAN.md | Markdown | 1 | Bu dosya (hazır) |
| P3 | 00-metodoloji.md | Markdown | 1 | Genel metodoloji açıklaması |
| P4 | 01-nist-csf-2-uyarlama.md | Markdown | 1–2 | NIST CSF 2.0'ın K-12'ye uyarlanması |
| P5 | 02-kvkk-okullar-icin.md | Markdown | 2 | KVKK'nın okul bağlamında yorumu |
| P6 | 03-meb-rehberi-eslestirme.md | Markdown | 2 | MEB rehberleri ile çapraz eşleştirme |
| P7 | NIST-CSF-2-K12-Olgunluk.xlsx | Excel | 1–2 | Olgunluk değerlendirme şablonu (tüm K-12 kullanabilir) |
| P8 | KVKK-Uyum-Checklist.xlsx | Excel | 2 | KVKK uyum kontrol listesi (okullara özel) |
| P9 | Risk-Register-Sablon.xlsx | Excel | 2 | Risk envanteri şablonu |
| P10 | Iyilestirme-Yol-Haritasi.xlsx | Excel | 4 | Kısa/orta/uzun vade roadmap şablonu |
| P11 | Olay-Mudahale-Plani-Sablon.docx | Word | 4 | K-12 için olay müdahale planı şablonu |
| P12 | Yetkilendirme-Belgesi-Sablon.docx | Word | 1 | Yetkilendirme belgesi şablonu (kişisel veriler kaldırılmış) |
| P13 | k12-network-mevcut-jenerik.png | PNG/SVG | 3 | Jenerik mevcut durum mimarisi (anonim) |
| P14 | k12-network-hedef-jenerik.png | PNG/SVG | 4 | Jenerik hedef mimari |
| P15 | 04-iyilestirme-yol-haritasi.md | Markdown | 4 | Yol haritası anlatım metni |
| P16 | 05-quick-wins.md | Markdown | 1 | Her okulun bugün yapabileceği 10 hızlı kazanım |
| P17 | case-study/00-baglam.md | Markdown | 5 | Vaka çalışması girişi |
| P18 | case-study/01-mevcut-durum.md | Markdown | 5 | Anonim mevcut durum analizi |
| P19 | case-study/02-bulgular.md | Markdown | 5 | Anonim bulgular ve risk dereceleri |
| P20 | case-study/03-sonuclar.md | Markdown | 5 | Sonuçlar, öğrenimler, sınırlamalar |

### 🔒 Okul içi (REPO'YA GİTMEYECEK)

| # | Teslim Edilecek | Format | Hafta | Açıklama |
|---|---|---|---|---|
| G1 | Yetkilendirme_Belgesi_İmzalı.pdf | PDF (imzalı) | 1 | Müdür imzalı belge — okul arşivi |
| G2 | Donanım-Envanteri-Hüyük.xlsx | Excel | 2 | Tüm cihazların marka, model, MAC, IP listesi |
| G3 | Network-Diagram-Hüyük.drawio | draw.io | 2 | Okulun gerçek ağ topolojisi |
| G4 | Yapilandirma-Notlari.docx | Word | 3 | Switch/router config notları |
| G5 | Nmap-Sonuclari-AAAA-AA-GG.txt | Text | 3 | Aktif tarama sonuçları |
| G6 | Zafiyet-Listesi-Detay-Hüyük.xlsx | Excel | 3 | Bulunan zafiyetler, gerçek IP/host adlarıyla |
| G7 | NIST-CSF-Olgunluk-Skor-Hüyük.xlsx | Excel | 4 | Hüyük için doldurulmuş olgunluk skoru |
| G8 | KVKK-Uyum-Hüyük.xlsx | Excel | 4 | Hüyük için doldurulmuş KVKK durumu |
| G9 | Detayli-Rapor-Hüyük.docx | Word | 5 | Okula teslim edilecek tam rapor |
| G10 | Yonetici-Ozeti-Sunum.pptx | PowerPoint | 5 | Müdüre sunum (15-20 dk) |
| G11 | Yol-Haritasi-Hüyük.xlsx | Excel | 5 | Spesifik öneriler + tahmini maliyet/etki |

---

## Haftalık Kontrol Noktaları

### Hafta 1: Hazırlık (13–20 Mart)
- [ ] Yetki belgesi müdür tarafından imzalanmış
- [ ] NIST CSF 2.0 dokümantasyonu çalışılmış
- [ ] CIS Controls v8 IG1 listesi anlaşılmış
- [ ] KVKK'nın eğitim sektörü hükümleri özetlenmiş
- [ ] MEB BTSB güncel rehberi okunmuş
- [ ] Public repo iskeleti GitHub'a yüklenmiş (placeholder dokümanlarla)

### Hafta 2: Veri Toplama I (21–27 Mart)
- [ ] Tüm fiziksel cihazlar envantere alındı (G2)
- [ ] Network topoloji diyagramı çıkarıldı (G3)
- [ ] Mevcut güvenlik politikaları (varsa) toplandı
- [ ] WiFi yapılandırması belgelendi
- [ ] Kullanıcı/grup yapısı dökümante edildi

### Hafta 3: Veri Toplama II (28 Mart – 4 Nisan)
- [ ] Switch/router yapılandırmaları read-only çekildi (G4)
- [ ] Aktif tarama mesai dışı yapıldı (G5) — Nmap + opsiyonel zafiyet scanner
- [ ] KVKK kontrol listesi doldurulmaya başlandı
- [ ] Pasif trafik gözlemi (1-2 saatlik örnek) alındı

### Hafta 4: Değerlendirme (5–12 Nisan)
- [ ] NIST CSF 2.0'ın 6 fonksiyonu için olgunluk skoru hesaplandı (G7)
- [ ] Tüm bulgular risk derecesine göre sıralandı (G6)
- [ ] KVKK uyum tablosu tamamlandı (G8)
- [ ] Hedef mimari diyagramı çizildi (P14)
- [ ] İyileştirme yol haritası taslağı çıkarıldı

### Hafta 5: Raporlama (13–19 Nisan)
- [ ] Detaylı rapor (G9) tamamlandı ve müdüre teslim edildi
- [ ] Yönetici sunumu (G10) hazırlandı ve sunuldu
- [ ] Anonim vaka çalışması yazıldı (P17–P20)
- [ ] GitHub repo'su tamamen public hale getirildi
- [ ] LinkedIn paylaşımı hazırlandı

---

## Kritik Riskler ve Azaltma

| Risk | Azaltma |
|---|---|
| Aktif tarama eğitim faaliyetlerini etkiler | Yalnızca hafta sonu / mesai dışı; pasif yöntemleri önceliklendir |
| Müdür izin geç verir / vermez | Hibrit plana geç — yalnızca pasif gözlem + dokümantasyon + jenerik vaka çalışması |
| Bulgular GitHub'a sızar | Her commit öncesi `git diff` kontrolü; gerçek isim/IP filtresi |
| Çalışma süresi taşar | Quick wins'i önce yayınla; vaka çalışmasını sonraya bırak |
| Yıl sonu sınav haftalarıyla çakışır | Hafta 3'teki aktif taramayı sınav haftası dışına al |

---

## Başarı Kriterleri

Bu proje şu çıktılar elde edildiğinde başarılı sayılır:

1. ✅ Okul yönetimi, bilgi güvenliği seviyesi hakkında somut bir rapor sahibi
2. ✅ Önceliklendirilmiş bir iyileştirme yol haritası tanımlanmış
3. ✅ KVKK uyum durumu belgelenmiş
4. ✅ Türkiye'deki diğer K-12 okulları için yeniden kullanılabilir şablonlar yayınlanmış
5. ✅ LinkedIn üzerinden paylaşılmış, en az 10 sektör profesyonelinden geri bildirim alınmış
