<div align="center">

# 🎫 ts-ticket

<p align="center">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/Discord.js-5865F2?style=for-the-badge&logo=discord&logoColor=white"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/>
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/abdulrahmanqdev/ts-ticket?style=flat-square&color=yellow"/>
  <img src="https://img.shields.io/github/forks/abdulrahmanqdev/ts-ticket?style=flat-square&color=green"/>
  <img src="https://img.shields.io/github/last-commit/abdulrahmanqdev/ts-ticket?style=flat-square&color=orange"/>
</p>

<p align="center">
  <strong>TypeScript ile geliştirilmiş Discord ticket sistemi.</strong><br/>
  Buton tabanlı ticket açma/kapama, komut ve event handler yapısıyla tam donanımlı bot altyapısı.
</p>

</div>

---

## 📖 Genel Bakış

**ts-ticket**, TypeScript kullanılarak geliştirilmiş bir Discord ticket botudur. Kullanıcılar buton aracılığıyla destek talebi (ticket) açabilir, moderatörler ise bu talepleri yönetebilir. Modüler yapısıyla kolayca genişletilebilir.

---

## ✨ Özellikler

- 🎫 Buton ile ticket açma ve kapatma
- 🔧 Slash komut desteği
- 📡 Event handler sistemi
- 🗂️ Modüler handler yapısı (komutlar, butonlar, eventler)
- 🚀 Deploy komutlarını otomatik kaydet
- 🔒 Tam TypeScript tip güvenliği

---

## 🛠️ Teknoloji Yığını

| Teknoloji | Amaç |
|---|---|
| TypeScript | Dil |
| Discord.js | Discord API Kütüphanesi |
| Node.js | Çalışma Ortamı |

---

## 🚀 Başlarken

### Gereksinimler
- Node.js `>= 18.x`
- [Discord Developer Portal](https://discord.com/developers/applications) üzerinden bir bot token'ı

### Kurulum

```bash
git clone https://github.com/abdulrahmanqdev/ts-ticket.git
cd ts-ticket
npm install
```

### Yapılandırma

`src/config.ts` dosyasına bot bilgilerini gir:

```ts
export default {
  token: "BOT_TOKEN_BURAYA",
  clientId: "CLIENT_ID_BURAYA",
  guildId: "GUILD_ID_BURAYA",
}
```

### Slash Komutlarını Deploy Et

```bash
npx ts-node src/utils/deployCommands.ts
```

### Çalıştır

```bash
npx ts-node src/utils/index.ts
```

---

## 📁 Proje Yapısı

```
ts-ticket/
├── src/
│   ├── buttons/
│   │   ├── closeTicket.ts       # Ticket kapatma butonu
│   │   └── createTicket.ts      # Ticket oluşturma butonu
│   ├── commands/
│   │   └── ticket.ts            # Ticket slash komutu
│   ├── events/
│   │   ├── interactionCreate.ts # Etkileşim olayı
│   │   └── ready.ts             # Bot hazır olayı
│   ├── handlers/
│   │   ├── loadButtons.ts       # Buton yükleyici
│   │   ├── loadCommands.ts      # Komut yükleyici
│   │   └── loadEvents.ts        # Event yükleyici
│   └── utils/
│       ├── deployCommands.ts    # Slash komut deploy
│       ├── config.ts            # Bot yapılandırması
│       └── index.ts             # Ana giriş noktası
├── tsconfig.json
├── package.json
└── LICENSE
```

---

## 🤝 Katkıda Bulunma

1. Repoyu fork'la
2. Yeni dal oluştur (`git checkout -b ozellik/yeni-ozellik`)
3. Değişiklikleri kaydet ve Pull Request aç

---

## 👤 Geliştirici

**@abdulrahmanqdev**

