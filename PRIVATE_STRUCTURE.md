# Okul İçi (Gizli) Klasör Yapısı

> ⚠️ **Bu dosya repo'da bilgi amaçlı bulunur ama buradaki klasör yapısı yalnızca local'de tutulur. GitHub'a kesinlikle commit edilmez.**

## Önerilen Local Konum

```
~/Documents/Hüyük-Bilgi-Guvenligi-Ozel/   ← GitHub klasörünün DIŞINDA
```

Bu klasör, GitHub repo'sundan tamamen ayrı tutulmalıdır. Repo klasörü `Desktop/k12-cybersecurity/`, gizli klasör `Documents/Hüyük-Bilgi-Guvenligi-Ozel/` gibi. Aralarında symlink, alt klasör veya kısayol bulunmamalıdır.

## Klasör Yapısı

```
Hüyük-Bilgi-Guvenligi-Ozel/
│
├── 00-yetkilendirme/
│   └── Yetkilendirme_Belgesi_İmzalı.pdf   ← Müdür imzalı taranmış halde
│
├── 01-envanter/
│   ├── Donanim-Envanteri-Hüyük.xlsx        ← Tüm cihazlar (router, switch, AP, PC, smartboard, vb.)
│   ├── Yazilim-Envanteri-Hüyük.xlsx        ← Kurulu yazılımlar, sürümleri
│   └── Network-Diagram-Hüyük.drawio        ← Gerçek ağ topolojisi
│
├── 02-veri-toplama/
│   ├── 2026-03-21-nmap-sonuclari.txt       ← Aktif tarama çıktıları
│   ├── 2026-03-22-zafiyet-tarama.xml       ← OpenVAS/Nessus çıktısı
│   ├── 2026-03-23-wireshark-ornek.pcap     ← Pasif trafik örneği (1-2 saat)
│   ├── 2026-03-24-switch-config.txt        ← Read-only çekilmiş yapılandırma
│   ├── 2026-03-24-router-config.txt
│   └── 2026-03-25-wifi-config-notlar.docx
│
├── 03-degerlendirme/
│   ├── NIST-CSF-Olgunluk-Skor-Hüyük.xlsx   ← 6 fonksiyon × tier skorlaması
│   ├── KVKK-Uyum-Hüyük.xlsx                ← KVKK kontrol listesi (doldurulmuş)
│   ├── CIS-IG1-Hüyük.xlsx                  ← CIS Controls v8 IG1 durumu
│   └── Zafiyet-Listesi-Detay-Hüyük.xlsx    ← Bulunan zafiyetler, gerçek host adlarıyla
│
├── 04-rapor/
│   ├── Detayli-Rapor-Hüyük.docx            ← Müdüre teslim edilecek tam rapor
│   ├── Yonetici-Ozeti-Sunum.pptx           ← 15-20 dk sunum
│   ├── Yol-Haritasi-Hüyük.xlsx             ← Önerilerin maliyet/etki/efor matrisi
│   └── Iletisim-Kontrol-Notu.docx          ← Yayına teslimat öncesi son onay belgesi
│
├── 05-takip/
│   ├── Iyilestirme-Takip-Cizelgesi.xlsx    ← Önerilerin uygulanma durumu
│   └── Aylik-Inceleme-Notlari.md           ← Proje sonrası izleme
│
└── 99-arsiv/
    └── (eski versiyonlar)
```

## Bu Klasörü Nasıl Korumalısın

1. **iCloud / Google Drive senkronizasyonu** — bu klasörü bulut yedeklemesine al ama paylaşımdan koru (sadece kendi hesabın erişebilsin).

2. **Şifreli yedek** — kritik dosyaları (özellikle G5, G6 nolu çıktıları) parolalı bir ZIP veya 7Z arşivinde tut. Mac'te: `tar -czf - klasör | openssl enc -aes-256-cbc -salt -out arsiv.tar.gz.enc`

3. **Okul içi yedek** — proje sonunda **G9 (rapor)** ve **G10 (sunum)** dosyalarının birer kopyası okul yönetiminin arşivinde de bulunmalı. Bu, projenin sürdürülebilirliği ve devir teslim açısından önemli.

4. **Veri saklama süresi** — KVKK madde 7 uyarınca, taraması içeren teknik veriler (G5, G6) belirli bir saklama süresinin ardından silinmeli. 1-2 yıl sonra arşivleme veya silme planlanmalı.

## GitHub'a Yanlışlıkla Sızmayı Önle

`.gitignore` dosyana bu satırları ekle (zaten ekledim, ama hatırlatma):

```
# Hiçbir gizli klasör/dosya commit edilmesin
*-Hüyük.*
*-private.*
*-internal.*
**/private/
**/internal/
nmap-sonuclari*.txt
**.pcap
*-config.txt
```

Her commit öncesi mutlaka şu komutu çalıştır:

```bash
git status
git diff --cached  # commit'lenecekleri gözden geçir
```

Eğer içeri okul adı, gerçek IP, host adı vb. sızmış görünüyorsa **commit ETME**, önce temizle.

## Acil Durum: Sızma Olursa Ne Yapılır

Eğer hassas veri yanlışlıkla commit edilirse:

1. Commit'i hemen geri al: `git reset --soft HEAD~1`
2. Eğer push'lanmışsa hızlıca `git filter-repo` ile sil ve force push
3. Maruz kalan veri kritikse (gerçek zafiyet detayları) müdürü bilgilendir
4. GitHub support'tan **cache invalidation** talep et (GitHub forklar ve cache'leri tutar)

Önleme her zaman daha kolay — commit öncesi her seferinde dosyaları gözden geçir.
