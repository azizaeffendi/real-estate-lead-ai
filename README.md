<div align="center">

# 🏠 Real Estate Lead AI

**Sistem AI untuk agen properti — lead generation, scoring, WhatsApp bot, follow-up & CRM otomatis**

[![WhatsApp](https://img.shields.io/badge/WhatsApp-Bot-25D366?style=for-the-badge&logo=whatsapp)](https://whatsapp.com)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-412991?style=for-the-badge&logo=openai)](https://openai.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)
[![Made in Indonesia](https://img.shields.io/badge/Made%20in-Indonesia-red?style=for-the-badge)](https://github.com/azizaeffendi)

<br/>

> **Agen properti terbaik bukan yang punya listing terbanyak — tapi yang paling cepat follow up dan paling konsisten nurture lead. AI menggantikan tugas itu 24/7.**

```
LEAD FUNNEL DENGAN AI:

Awareness          Interest           Decision           Close
────────           ────────           ────────           ─────
Iklan IG/FB   →   WA Bot greet   →   Follow-up seq  →   Closing
Google Ads    →   AI qualification→  Virtual tour   →   Contract
Tokedia Rumah →   Lead scoring   →   Document prep  →   Referral
Rumah123      →   CRM entry      →   Negotiation AI →   Testimonial

Tanpa AI: 20% lead di-follow up, 3 hari response time
Dengan AI: 100% lead di-contact, < 5 menit response time
```

</div>

---

## 🎯 Masalah Utama Agen Properti

```
❌ TANPA AI:
- Follow up manual → banyak lead hilang
- Tidak bisa handle ratusan inquiry sekaligus
- Kualifikasi lead membuang waktu (many unqualified)
- Listing description butuh 1-2 jam per properti
- Sulit track history percakapan dengan semua prospek

✅ DENGAN SISTEM INI:
- Bot WA handle semua inquiry 24/7
- AI kualifikasi lead otomatis (budget? timeline? ready to buy?)
- Scoring: hot/warm/cold → prioritaskan yang mana dulu
- Auto-generate listing description dari foto + spesifikasi
- CRM otomatis update setiap interaksi
```

---

## 🤖 AI WhatsApp Lead Handler

### Alur Percakapan Otomatis

```
Prospek: "Halo, ada info rumah di Depok?"

Bot: "Halo! Saya bantu carikan properti yang cocok 😊
      Beberapa pertanyaan singkat ya:
      
      1️⃣ Budget Anda sekitar berapa?
         A) < 500 juta
         B) 500jt - 1 M
         C) > 1 Miliar"

Prospek: "B"

Bot: "Oke, budget 500jt-1M di Depok!
      Preferensi tipe properti?
      A) Rumah tapak
      B) Apartemen
      C) Ruko"
      
[... setelah 3-4 pertanyaan ...]

Bot: "Baik! Berdasarkan kriteria Anda, saya temukan 3 pilihan:

     🏠 Cluster Modern Depok - 3KT/2KM - Rp 750jt
     🏠 Perumahan Grand Sawangan - 2KT/1KM - Rp 520jt  
     🏠 Townhouse Premium - 3KT/3KM - Rp 890jt
     
     Mau info detail atau jadwal survey?"

[Data lead otomatis masuk ke CRM + notif ke agen]
```

---

## 📊 Lead Scoring Engine

```python
def score_lead(lead_data):
    score = 0
    
    # Budget readiness (max 30 poin)
    if lead_data.budget_confirmed:     score += 30
    elif lead_data.budget_range:       score += 15
    
    # Timeline (max 25 poin)
    if lead_data.timeline == "1_month":   score += 25
    elif lead_data.timeline == "3_month": score += 15
    elif lead_data.timeline == "6_month": score += 8
    
    # Engagement (max 20 poin)
    score += min(lead_data.message_count * 2, 20)
    
    # Pre-approval (max 15 poin)
    if lead_data.has_kpr_preapproval:  score += 15
    
    # Referral (max 10 poin)
    if lead_data.source == "referral": score += 10
    
    # Classify
    if score >= 60: return "HOT 🔥"
    elif score >= 35: return "WARM 🌡️"
    else: return "COLD ❄️"
```

---

## 📝 AI Listing Generator

```
INPUT (dari agen):
- Foto properti (5-10 foto)
- Spesifikasi: LT, LB, KT, KM, lokasi, fasilitas
- Harga

OUTPUT AI:
1. Judul listing yang compelling (SEO-optimized)
2. Deskripsi panjang 300-500 kata dengan:
   - Highlight lokasi strategis
   - Benefit lingkungan sekitar
   - Fasilitas yang menonjol
   - Investment potential
3. Short caption untuk Instagram/TikTok
4. Bullet points untuk marketplace properti
5. Hashtag 20+ untuk sosmed

WAKTU: 30 detik vs 1-2 jam manual
```

---

## 📁 Struktur

```
real-estate-lead-ai/
├── src/
│   ├── bot/                # WhatsApp lead bot
│   ├── scoring/            # Lead scoring engine
│   ├── listing-ai/         # Property description generator
│   ├── crm/                # CRM integration
│   └── follow-up/          # Automated follow-up sequences
├── docs/
│   ├── SETUP.md
│   └── LEAD-MANAGEMENT.md
└── examples/
    ├── residential/
    └── commercial/
```

---

## 📜 Lisensi
MIT © [azizaeffendi](https://github.com/azizaeffendi)

<div align="center">
**Muhammad Aziz A Effendi** · AI Marketing Engineer · Indonesia
[![GitHub](https://img.shields.io/badge/GitHub-@azizaeffendi-181717?style=flat-square&logo=github)](https://github.com/azizaeffendi)
</div>