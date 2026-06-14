# 🧠 ERIF AI v3.0 Ultimate

AI Tutor STEM Percuma untuk Pelajar Malaysia dengan integrasi lengkap AI percuma.

![Version](https://img.shields.io/badge/version-3.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Python](https://img.shields.io/badge/python-3.8+-yellow)

## ✨ Ciri-Ciri Lengkap

| Ciri | Status | Keterangan |
|------|--------|------------|
| 🤖 **Ollama** | ✅ Percuma | Local LLM (Llama3.2, Mistral, Qwen) - Tiada API Key |
| 🌐 **Kimi API** | ✅ | Moonshot AI untuk context panjang |
| 🎨 **Fooocus** | ✅ Percuma | Unlimited local image generation |
| 🖼️ **Pollinations** | ✅ Percuma | Online AI image (backup) |
| 📺 **yt-dlp** | ✅ Percuma | Download video YouTube, TikTok, IG, X |
| 🎙️ **Whisper** | ✅ Percuma | Transcribe audio/video BM |
| 📄 **Export** | ✅ | DOCX & PDF generator |
| 📊 **Plausible** | ✅ | Privacy analytics |

## 🚀 Cara Guna

### 1. Deploy Streamlit Cloud (Percuma)
[![Deploy to Streamlit](https://img.shields.io/badge/Deploy-Streamlit-red)](https://share.streamlit.io)

1. Fork repo ini
2. Pergi [share.streamlit.io](https://share.streamlit.io)
3. Connect GitHub & deploy

### 2. Run Local

```bash
# Install dependencies
pip install -r requirements.txt

# Jalankan
streamlit run erif_v3_complete.py
```

## 🎯 Commands

### Chat Biasa
```
"Apa itu photosintesis?"
"Terangkan hukum Newton"
```

### Python Code
```
"Plot graf y=sin(x)"
"Kira luas segitiga dengan base 10, height 5"
```

### Generate Image
```
"Lukis atom karbon 3D"
"Gambar peta minda sejarah Malaya"
```

### Download Video
```
"Download https://youtube.com/watch?v=..."
"Simpan video TikTok ini https://vt.tiktok.com/..."
```

### Transcribe
1. Upload fail audio/video (MP3, MP4, WAV)
2. Taip: `"transcribe"` atau `"transkrip"`

### Export
```
"Buat nota bab Geografi, export PDF"
"Simpan nota ini dalam Word"
```

## ⚙️ Setup Ollama (Percuma - Tiada API Key)

```bash
# 1. Install Ollama
https://ollama.com/download

# 2. Download model
ollama pull llama3.2

# 3. Start server
ollama serve

# 4. Toggle "Guna Ollama" dalam sidebar ERIF
```

## 🎨 Setup Fooocus (Unlimited Image Percuma)

```bash
# 1. Clone Fooocus
git clone https://github.com/lllyasviel/Fooocus.git
cd Fooocus

# 2. Install & run
python entry_with_update.py --listen

# 3. Toggle Fooocus dalam ERIF sidebar
```

## 📋 Keperluan Sistem

- Python 3.8+
- 4GB RAM minimum
- Internet untuk online features
- GPU (optional) untuk Fooocus cepat

## 🔧 Environment Variables

```bash
# Optional: Plausible Analytics
PLAUSIBLE_DOMAIN=erif-ai.streamlit.app
PLAUSIBLE_SCRIPT=https://plausible.io/js/script.js

# Optional: Default API Key
KIMI_API_KEY=sk-xxx
```

## 📁 Struktur Fail

```
ERIF AI/
├── erif_v3_complete.py    # Main application
├── requirements.txt         # Dependencies
├── README.md               # This file
└── .streamlit/
    └── config.toml         # UI config
```

## 🤝 Integrasi API Percuma

| Servis | Penggunaan | Limit |
|--------|-----------|-------|
| Ollama | Chat AI | Unlimited (local) |
| Fooocus | Image Gen | Unlimited (local) |
| Pollinations | Image Gen | Unlimited |
| Whisper | Transcribe | Unlimited (local) |
| yt-dlp | Video Download | Unlimited |
| Kimi API | Chat (optional) | Bergantung API key |

## 🐛 Troubleshooting

| Masalah | Penyelesaian |
|---------|-------------|
| Ollama tidak connect | Pastikan `ollama serve` berjalan |
| Fooocus tidak connect | Check URL dalam sidebar (default: http://127.0.0.1:7865) |
| Whisper error | Install: `pip install openai-whisper` |
| yt-dlp error | Install: `pip install yt-dlp` |

## 📜 License

MIT License - Guna dengan bebas untuk pendidikan!

---

**Dibuat dengan ❤️ untuk pelajar Malaysia**
