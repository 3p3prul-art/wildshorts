# WildShorts — AI Content Creator
YouTube Shorts generator for outdoor adventure content, powered by Claude AI.

## Deploy ke Vercel (5 menit)

### 1. Upload folder ini ke GitHub
- Buat repo baru di github.com
- Upload semua file dalam folder ini (index.html, vercel.json, api/chat.js)

### 2. Connect ke Vercel
- Buka vercel.com → New Project
- Import repo GitHub kamu
- Klik Deploy (settings default sudah benar)

### 3. Set API Key (WAJIB)
- Di Vercel dashboard → Project → Settings → Environment Variables
- Tambahkan:
  - Name:  ANTHROPIC_API_KEY
  - Value: sk-ant-xxxxxx (API key kamu dari console.anthropic.com)
- Klik Save → lalu Redeploy

### 4. Done!
Website langsung bisa diakses siapa saja. User TIDAK perlu input API key.

---

## Struktur File
```
wildshorts/
├── index.html        ← Frontend (semua UI)
├── vercel.json       ← Konfigurasi Vercel
└── api/
    └── chat.js       ← Serverless function (proxy ke Anthropic)
```

## Fitur
- 💡 Generate ide konten (5 ide per generate)
- 🏷 Generate judul (5 opsi) + 30 hashtag
- 🎬 Generate scene breakdown + AI video prompts
- 🌙 Dark / Light mode
- 🌐 Bahasa EN / ID
- 👤 Login username
- 💾 History (tersimpan di browser)
- 🖨 Export PDF
- 📝 Copy for Notion

## Mendapatkan Anthropic API Key
1. Buka console.anthropic.com
2. Daftar / login
3. API Keys → Create Key
4. Copy dan paste ke Vercel Environment Variables
