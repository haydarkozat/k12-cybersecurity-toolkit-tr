# K-12 Okul Siber Güvenlik Değerlendirmesi

> **NIST Cybersecurity Framework 2.0 ve KVKK uyumluluğu üzerine kurulu, bir Türk devlet ortaokulunda gerçekleştirilen bilgi güvenliği olgunluk değerlendirmesi.**
>
> *A cybersecurity maturity assessment of a Turkish public middle school, grounded in NIST CSF 2.0 and Turkish data protection law (KVKK).*

[![NIST CSF 2.0](https://img.shields.io/badge/Framework-NIST%20CSF%202.0-1f6feb.svg)](https://www.nist.gov/cyberframework)
[![KVKK](https://img.shields.io/badge/Compliance-KVKK-d62c2c.svg)](https://www.kvkk.gov.tr)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 🇬🇧 In One Paragraph

This project documents a structured information security posture assessment of a 250-user K-12 public middle school in Türkiye, conducted by the school's IT coordinator. It applies NIST Cybersecurity Framework 2.0 — including the new **Govern** function — to a context most security frameworks aren't designed for: small, resource-constrained educational institutions operating within a centralized state education hierarchy. The methodology, anonymized findings, KVKK compliance checklist and improvement roadmap are designed to be **reusable by any K-12 school IT coordinator** in Türkiye.

---

## 🎯 Proje Amacı

Türkiye'deki okulların bilgi güvenliği büyük ölçüde belgelenmemiş bir alandır. Bilişim sorumluları çoğu zaman teknik kontrolleri sezgisel olarak uygular, ancak:

- Uluslararası bir çerçeveyle hizalı bir olgunluk seviyesi ölçümü yoktur
- KVKK uyumluluğu net şekilde belgelenmemiştir
- Yönetime aktarılabilecek standart bir risk envanteri yoktur
- Diğer okullarla karşılaştırılabilir bir benchmark eksiktir

Bu çalışma, **bir okulda yapılan değerlendirmenin metodolojisini ve şablonlarını açık kaynak olarak yayınlayarak** Türkiye'deki diğer K-12 bilişim sorumlularına yeniden kullanılabilir bir kaynak sunar.

## 🏛️ Bağlam: Türkiye'de K-12 Bilgi Güvenliği

Türk devlet okulları ilginç bir güvenlik bağlamında çalışır:

- **Merkezi sistemler** (e-Okul, MEBBİS, DYS) MEB tarafından korunur — yerel kapsam dışında
- **Yerel ağ** (modem, switch, AP, sınıf cihazları, Fatih Projesi etkileşimli tahtaları) okul tarafından yönetilir
- **Bilişim sorumlusu** çoğunlukla branş öğretmenidir, tam zamanlı BT personeli değildir
- **Bütçe ve donanım kısıtları** ileri düzey güvenlik çözümlerini erişilemez kılar
- **KVKK öğrenci verisi** açısından okulu doğrudan veri sorumlusu konumuna yerleştirir

Bu çerçevede "kurumsal güvenlik" yaklaşımları (ISO 27001 sertifikası, kurumsal SIEM çözümleri) gerçekçi değildir. Bu proje, **gerçek kısıtlar altında ne yapılabileceğine** dair pragmatik bir yol önerir.

## 🧭 Metodoloji

Çalışma şu çerçevelerden yararlanır:

| Çerçeve | Rolü |
|---|---|
| **NIST Cybersecurity Framework 2.0** | Ana olgunluk değerlendirme çerçevesi (Govern, Identify, Protect, Detect, Respond, Recover) |
| **CIS Controls v8 IG1** | Küçük kuruluşlar için temel kontrol seti |
| **ISO/IEC 27001 Annex A** | Karşılaştırmalı kontrol eşleştirmesi |
| **KVKK** | Türkiye'de zorunlu hukuki uyum çerçevesi |
| **MEB Bilişim Güvenliği Rehberi** | Sektörel rehber |

## 📂 Repo Yapısı

```
.
├── README.md                          ← bu dosya
├── PROJECT_PLAN.md                    ← 5 haftalık plan + teslim edilecekler matrisi
├── PRIVATE_STRUCTURE.md               ← okul içi (gizli) klasör şablonu — REPO'DA TUTULMAZ
├── LICENSE                            ← MIT
├── .gitignore
│
├── docs/                              ← metodoloji ve çerçeve dokümanları
│   ├── 00-metodoloji.md
│   ├── 01-nist-csf-2-uyarlama.md
│   ├── 02-kvkk-okullar-icin.md
│   ├── 03-meb-rehberi-eslestirme.md
│   ├── 04-iyilestirme-yol-haritasi.md
│   └── 05-quick-wins.md
│
├── templates/                         ← yeniden kullanılabilir şablonlar
│   ├── Yetkilendirme-Belgesi-Sablon.docx
│   ├── NIST-CSF-2-K12-Olgunluk.xlsx
│   ├── KVKK-Uyum-Checklist.xlsx
│   ├── Risk-Register-Sablon.xlsx
│   ├── Iyilestirme-Yol-Haritasi.xlsx
│   └── Olay-Mudahale-Plani-Sablon.docx
│
├── case-study/                        ← anonimleştirilmiş vaka çalışması
│   ├── 00-baglam.md
│   ├── 01-mevcut-durum.md
│   ├── 02-bulgular.md
│   └── 03-sonuclar.md
│
├── diagrams/                          ← jenerik mimari diyagramlar
│   ├── k12-network-mevcut-jenerik.png
│   ├── k12-network-hedef-jenerik.png
│   └── nist-csf-2-fonksiyonlar.png
│
└── scripts/                           ← (opsiyonel) yardımcı araçlar
    └── README.md
```

## ⚠️ Gizlilik

Bu repoda hiçbir şekilde:
- Çalışmanın yapıldığı okulun adı, adresi, bölgesi
- Personel veya öğrenci kimlik bilgisi
- Spesifik IP planları, donanım marka/model bilgileri
- Tanımlanabilir log örnekleri veya ekran görüntüleri

bulunmaz. Vaka çalışmasında okul "Türkiye'de bir K-12 devlet ortaokulu" olarak genelleştirilmiştir.

## 📜 Lisans ve Atıf

MIT Lisansı altında yayınlanmıştır. Bu çalışmadaki şablonları ve metodolojiyi kendi okulunuzda kullanmak için herhangi bir izin almanıza gerek yoktur. Akademik atıf yapmak isterseniz:

```
Kozat, H. (2026). K-12 Okul Siber Güvenlik Değerlendirmesi:
NIST CSF 2.0'ın Türk Devlet Ortaokuluna Uyarlanması.
GitHub: github.com/haydarkozat/k12-cybersecurity-assessment
```

## 🤝 Katkıda Bulunma

Diğer okullardan gelen geri bildirimler, şablon iyileştirmeleri ve farklı okul tiplerine (lise, ilkokul, anaokulu) uyarlamalar memnuniyetle karşılanır. Issue açarak veya pull request göndererek katkıda bulunabilirsiniz.

---

📧 İletişim: LinkedIn üzerinden — [linkedin.com/in/haydar-kozat](https://linkedin.com/in/haydar-kozat)
