# 🚀 Discord Bot - Kurulum Rehberi

## 📦 GEREKSİZ BAĞLANTILAR

```bash
npm install discord.js
npm install @discordjs/rest
npm install @discordjs/voice
npm install discord-api-types
npm install dotenv
npm install ffmpeg-static
npm install openai
npm install play-dl
npm install yt-search
npm install ytdl-core
npm install @google/generative-ai
```

## 🔑 ORTAM DEĞİŞKENLERİ (.env)

Proje root'unda `.env` dosyası oluştur:

```
DISCORD_TOKEN=your_discord_bot_token_here
GEMINI_API_KEY=your_gemini_api_key_here
```

## 🎮 DISCORD BOT KURULUM

1. **Discord Developer Portal'a git:** https://discord.com/developers/applications
2. **"New Application" tıkla**
3. **Adını ver:** `Americans Roleplay Bot`
4. **"Bot" sekmesine git**
5. **"Add Bot" tıkla**
6. **Token kopyala** → `.env` dosyasına yapıştır

### İZİNLER (Scopes)
Bot kurulurken şunları seç:
- ✅ `bot`
- ✅ `applications.commands`

### İZİNLER (Permissions)
- ✅ Send Messages
- ✅ Read Messages/View Channels
- ✅ Manage Messages
- ✅ Embed Links
- ✅ Attach Files
- ✅ Read Message History
- ✅ Mention @everyone, @here, All Roles
- ✅ Use Slash Commands
- ✅ Manage Roles
- ✅ Manage Channels
- ✅ Kick Members
- ✅ Ban Members
- ✅ Create Public Threads
- ✅ Mute Members

### İNTENT SETTINGS
Bot Settings → Intents kısmında şunları aç:
- ✅ PRESENCE INTENT
- ✅ SERVER MEMBERS INTENT
- ✅ MESSAGE CONTENT INTENT
- ✅ GUILD MEMBERS INTENT

## 🚀 BOTU ÇALIŞTIR

```bash
node index.js
```

Çıktıda şunu görmelisin:
```
✅ Bot Americans Roleplay#4270 olarak giriş yaptı!
✅ Veriler yüklendi!
✅ Slash komutları başarıyla kaydedildi!
💚 Keep-alive heartbeat system started!
```

## 🌐 BOTu SUNUCUYA EKLE

1. Discord Developer Portal → Bot → OAuth2 → URL Generator
2. Scopes: `bot` + `applications.commands`
3. Permissions: (yukarıda listelenen tüm izinler)
4. Oluşturulan linke tıkla ve sunucuna davet et

## 📊 SUNUCU KURULUMU

Bot eklendikten sonra:

1. `/setup-logs #log-channel` - Log kanalı ayarla
2. `/welcome #welcome-channel` - Hoşgeldin kanalı ayarla
3. `/kurlg #report-channel` - Şikâyet kanalı ayarla
4. `/senkronizasyon` - Kanalları rollere göre senkronize et (ADMIN)

## 🔄 DATA PERSISTENCE

Bot otomatik olarak `data.json` dosyasında tüm verileri saklıyor.
Sunucu kapansa bile bot restart olunca tüm veriler geri yüklenir!

## 📝 DOSYA YAPISI

```
.
├── index.js              # Ana bot dosyası
├── data.json             # Verileri saklayan dosya
├── package.json          # Bağlantılar
├── .env                  # Ortam değişkenleri (gizli)
├── KOMUTLAR.md           # Tüm komutlar (bu dosya)
├── SETUP.md              # Kurulum rehberi (bu dosya)
└── replit.md             # Proje bilgileri
```

## 🆘 SORUN GİDERME

### "Bot token invalid" hatası
- Token'ı doğru kopyala
- `.env` dosyasında var mı kontrol et

### "DISCORD_TOKEN is not defined"
- `.env` dosyası oluştur
- `dotenv` package'i yükle: `npm install dotenv`

### Komutlar gözükmüyor
- Bot'u reboot et
- Bot token'ını sağla
- Intent'ler açık mı kontrol et

### Sunucuda çalışmıyor ama terminalde açık
- Bot invite linkini kontrol et
- Permissions'ları kontrol et
- Intent'leri Discord Developer Portal'da aç

## 🚀 DEPLOYMENT (REPLIT)

Replit'te 24/7 çalıştırmak için:

1. **"Publish" butonuna tıkla**
2. **"Deploy" seç**
3. Bot herkese açık olur ve her zaman online kalır

## 📱 MOBİL KULLANIM

Discord mobil uygulamasında tüm komutlar çalışır:
- Slash komutlar tam compat
- Butonlar çalışıyor
- Menu'ler çalışıyor

---

**Bot Geliştirici:** truesultan31-byte  
**Email:** truesultan31@gmail.com  

Sorular? Bot hatasını bulursam ne yapmalı? Hepsi rehberde! 👍

