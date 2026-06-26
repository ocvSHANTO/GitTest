<div align="center">

<br/>

<img src="https://img.shields.io/badge/Privacy%20Forge-v1.0.0-00d4ff?style=for-the-badge&logo=shield&logoColor=white" alt="Privacy Forge"/>

<br/><br/>

# 🛡️ Privacy Forge

### *Everything Privacy. Offline. No Upload. No Tracking.*

<br/>

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-Visit_Now-00d4ff?style=for-the-badge)](https://ocvshanto.github.io/privacy-forge)
[![License: MIT](https://img.shields.io/badge/License-MIT-7c3aed?style=for-the-badge)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/ocvSHANTO/privacy-forge?style=for-the-badge&color=f59e0b)](https://github.com/ocvSHANTO/privacy-forge/stargazers)
[![Made with HTML](https://img.shields.io/badge/Made_with-HTML%20%2F%20CSS%20%2F%20JS-10b981?style=for-the-badge)](https://github.com/ocvSHANTO/privacy-forge)
[![No Backend](https://img.shields.io/badge/Backend-None_(100%25_Offline)-ef4444?style=for-the-badge)]()

<br/>

> **Privacy Forge** is a comprehensive, offline-first browser-based privacy toolkit.  
> Every single operation runs **locally on your device** — nothing is uploaded, stored on servers, or tracked. Ever.

<br/>

![Privacy Forge Banner](https://via.placeholder.com/900x400/060a14/00d4ff?text=Privacy+Forge+%E2%80%94+13+Privacy+Tools%2C+Zero+Upload)

<br/>

</div>

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [🔧 Tools Overview](#-tools-overview)
- [🚀 Getting Started](#-getting-started)
- [📁 Project Structure](#-project-structure)
- [🛠 Tech Stack](#-tech-stack)
- [🔒 Privacy Guarantee](#-privacy-guarantee)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [👤 Developer](#-developer)

---

## ✨ Features

<table>
<tr>
<td>

- 🔒 **100% Offline First** — No internet required after loading
- 🚫 **Zero Data Collection** — Nothing is sent anywhere
- 📴 **No Account Required** — Open and use instantly
- 🆓 **Completely Free** — No paywalls, no subscriptions
- 📱 **Mobile Friendly** — Works great on phone & desktop
- ⚡ **Instant Results** — All processing is client-side
- 🔐 **AES-256-GCM Encryption** — Military-grade security
- 🎨 **Modern Dark UI** — Clean, beautiful interface

</td>
<td>

```
┌─────────────────────────────────┐
│       PRIVACY GUARANTEE         │
│                                 │
│  📡 Data Upload      →  ZERO   │
│  🍪 Tracking Cookies →  ZERO   │
│  📊 Analytics        →  ZERO   │
│  🔑 Account Needed   →  ZERO   │
│  💰 Cost             →  ZERO   │
│  🌐 Server Calls     →  ZERO   │
└─────────────────────────────────┘
```

</td>
</tr>
</table>

---

## 🔧 Tools Overview

### 🔑 1. Password Generator
> Generate cryptographically secure passwords using the **Web Crypto API**.

| Feature | Details |
|---------|---------|
| Strong Password | Custom length (8–128), character sets, no-similar option |
| Memorable Password | Word-based with leet substitution, symbols, numbers |
| PIN Generator | 4–10 digits, no-repeat, no-sequential options |
| Passphrase | Multiple words with custom separators, diceware-style |
| Custom Rules | Build your own character set from scratch |
| Strength Meter | Real-time visual strength + entropy score in bits |
| History | Last 10 generated passwords stored in-session |

---

### 📱 2. QR Forge
> A **complete QR toolkit** — not just a generator.

**QR Types Supported:**
```
🌐 Website URL          📶 Wi-Fi Password        👤 Contact (vCard)
📧 Email                📞 Phone Number          💬 SMS
💚 WhatsApp             ✈️ Telegram              📍 Location (Maps)
📅 Calendar Event       📝 Plain Text            ₿ Cryptocurrency
```

**Design Features:** Custom colors · Logo in center · SVG/PNG export · Error correction levels

**QR Decoder:** Upload any QR image → instantly decode content (uses browser BarcodeDetector API)

---

### 🖼️ 3. Metadata Cleaner + EXIF Viewer
> See what's hidden in your images. Then remove it.

- **EXIF Viewer** — Shows all metadata: GPS coordinates, camera model, device, software, timestamps
- **Sensitive field detection** — Highlights dangerous fields in red
- **One-click removal** — Strip all metadata from JPG, PNG, WebP
- **Batch processing** — Clean multiple images at once
- **Before/after comparison** — See exactly what was removed
- **Export JSON** — Save EXIF data report

---

### 🔗 4. URL Cleaner
> Remove tracking parameters before sharing links.

**Automatically removes 40+ tracking parameters:**
```
utm_source  utm_medium  utm_campaign  utm_term  utm_content
fbclid      gclid       msclkid       twclid    yclid
ref         si          mc_cid        mkt_tok   _hsenc
igshid      epik        spm           zanpid    ... and more
```
Also includes **URL Encode/Decode** utility built-in.

---

### 📝 5. Secure Note
> Write private notes with **AES-256-GCM** encryption.

```
Write Note → Set Password → Encrypt → Save / Export
Import File → Enter Password → Decrypt → Read / Edit
```

- Zero-knowledge: even if someone gets your file, they cannot read it without the password
- Export as `.encnote` file — importable anywhere
- Multiple notes stored in browser localStorage (encrypted)
- Password strength meter with PBKDF2 key derivation (310,000 iterations)

---

### 🔐 6. File Hash Generator
> Verify file integrity with cryptographic hashes.

| Algorithm | Bits | Security Status |
|-----------|------|-----------------|
| MD5 | 128-bit | ⚠️ Legacy (fast verification) |
| SHA-1 | 160-bit | ⚠️ Deprecated |
| SHA-256 | 256-bit | ✅ Secure |
| SHA-512 | 512-bit | ✅ Most Secure |

- **File Hash** — Drop any file, get all 4 hashes simultaneously
- **Text Hash** — Hash any text string
- **Verify Mode** — Paste expected hash → auto-detect algorithm → verify match/mismatch

---

### 🎲 7. Random Generator
> Cryptographically secure random data using `crypto.getRandomValues()`.

- **Random Password** — Custom charset, 8–128 characters
- **Recovery Codes** — 2FA-style backup codes (4–16 codes), downloadable as `.txt`
- **Security Token** — HEX / Base64 / AlphaNum API keys (16–64 bytes entropy)
- **UUID Generator** — v4 (random) and v1 (time-based), bulk generate 10 at once
- **OTP Secret** — Base32-encoded TOTP secret for Google Authenticator
- **Random Number** — Unbiased number in any custom range

---

### 🔠 8. Text Encoder / Decoder
> Multi-format encoding with live conversion.

| Format | Encode | Decode |
|--------|--------|--------|
| Base64 | ✅ | ✅ |
| URL Encoding | ✅ | ✅ |
| HTML Entities | ✅ | ✅ |
| Hexadecimal | ✅ | ✅ |
| Binary | ✅ | ✅ |
| ASCII Codes | ✅ | ✅ |
| Morse Code | ✅ | ✅ + 🔊 Audio |
| ROT/Caesar Cipher | ✅ | ✅ (adjustable 1–25 shift) |
| Text Transform | Reverse · Upper · Lower · Title · Alternating · Mirror | — |

---

### 📂 9. File Inspector
> Analyze any file without uploading it anywhere.

- **Magic Byte Detection** — Identify real file type from binary signature (not just extension)
- **MIME Type** — Accurate type detection
- **SHA-256 Hash** — Instant file fingerprint
- **Hex Preview** — First 64 bytes shown in hex
- **Export Report** — Download full inspection as `.txt`

---

### 🌐 10. Browser Privacy Report
> Understand your browser's privacy exposure.

Checks and scores 15+ privacy factors:
```
🍪 Cookies Enabled          💾 LocalStorage / SessionStorage
📡 WebRTC (IP Leak Risk)    📍 Geolocation API
📷 Camera / Mic API         🔔 Notification Permission
🖥 User Agent String         📐 Screen Resolution (fingerprint)
🌍 Browser Language          🕐 Timezone Detection
```
Gives a **Privacy Score out of 100** with color-coded risk levels.

---

### 🧹 11. Data Cleaner
> Clean messy text data with one click.

- Remove duplicate lines
- Remove empty/blank lines
- Trim extra whitespace
- Remove zero-width & invisible Unicode characters (`U+200B`, `U+FEFF`, etc.)
- Normalize Unicode (NFC)
- Sort lines alphabetically
- Convert to lowercase
- Remove punctuation
- Before/after diff view

---

### 📋 12. Clipboard Cleaner
> Manage clipboard safely.

- Read and display clipboard content
- Detect sensitive patterns (emails, phone numbers, credit card patterns)
- Clear clipboard with one click
- **Safe Copy** — Strips hidden/invisible characters before copying

---

### 📷 13. EXIF Viewer (Standalone)
> Same as Metadata Cleaner — dedicated EXIF inspection view with JSON export.

---

## 🚀 Getting Started

### Option 1 — Use Online (Recommended)
Visit: **[https://ocvshanto.github.io/privacy-forge](https://ocvshanto.github.io/privacy-forge)**

No installation, no account, opens instantly in browser.

---

### Option 2 — Run Locally

```bash
# Clone the repository
git clone https://github.com/ocvSHANTO/privacy-forge.git

# Navigate into the project
cd privacy-forge

# Open in browser — no build step needed!
# On macOS:
open index.html

# On Linux:
xdg-open index.html

# On Windows:
start index.html
```

> ✅ No `npm install`, no build tools, no dependencies — just open `index.html`.

---

### Option 3 — Download ZIP

1. Click the green **Code** button on this page
2. Select **Download ZIP**
3. Extract the folder
4. Open `index.html` in any modern browser

---

## 📁 Project Structure

```
privacy-forge/
│
├── 📄 index.html                     ← Main landing page (start here)
│
├── 🔑 password-generator/
│   └── index.html                    ← Password Generator tool
│
├── 📱 qr-forge/
│   └── index.html                    ← QR Code Generator + Decoder
│
├── 🖼️  metadata-cleaner/
│   └── index.html                    ← EXIF Viewer + Metadata Cleaner
│
├── 🔗 url-cleaner/
│   └── index.html                    ← URL Tracking Parameter Remover
│
├── 📝 secure-note/
│   └── index.html                    ← AES-256 Encrypted Notes
│
├── 🔐 file-hash/
│   └── index.html                    ← File Hash Generator & Verifier
│
├── 🎲 random-generator/
│   └── index.html                    ← Cryptographic Random Data Generator
│
├── 🔠 text-encoder/
│   └── index.html                    ← Multi-format Text Encoder/Decoder
│
├── 📂 file-inspector/
│   └── index.html                    ← File Inspector + Browser Privacy + Data Cleaner
│
├── 📄 README.md                      ← This file
├── 📄 LICENSE                        ← MIT License
└── 📄 .gitignore                     ← Git ignore rules
```

---

## 🛠 Tech Stack

```
Frontend Only — No Backend Required
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Language        → HTML5 + CSS3 + Vanilla JavaScript (ES2022+)
Encryption      → Web Crypto API (AES-256-GCM, PBKDF2, SHA-256)
Randomness      → crypto.getRandomValues() — cryptographically secure
QR Code         → QRCode.js (loaded from cdnjs.cloudflare.com)
QR Decoding     → Browser BarcodeDetector API (Chrome/Edge)
File Reading    → FileReader API + ArrayBuffer
Storage         → localStorage (Secure Note only, encrypted)
Zero tracking   → No Google Analytics, no pixels, no cookies
Zero backend    → No Node.js, no PHP, no server whatsoever
```

---

## 🔒 Privacy Guarantee

Privacy Forge was built with one principle: **your data never leaves your device.**

| What happens to your data | Answer |
|--------------------------|--------|
| Files you drop/upload | Processed in RAM, never sent anywhere |
| Passwords you generate | Generated locally, never logged |
| Notes you encrypt | Stored in your browser's localStorage, encrypted |
| Hashes you compute | Computed in browser using Web Crypto API |
| URLs you clean | Processed client-side, not logged |
| Browser data checked | Read locally, never transmitted |

**External requests made by this app:** Only one — QRCode.js library from `cdnjs.cloudflare.com` when the QR tool is used. Everything else is self-contained.

---

## 🤝 Contributing

Contributions are welcome! Here's how to get involved:

```bash
# 1. Fork this repository (top-right button on GitHub)

# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/privacy-forge.git

# 3. Create a new branch for your feature
git checkout -b feature/your-feature-name

# 4. Make your changes — no build step needed

# 5. Commit with a clear message
git commit -m "feat: add [your feature name]"

# 6. Push to your fork
git push origin feature/your-feature-name

# 7. Open a Pull Request on GitHub
```

### 📌 Contribution Ideas

- [ ] Add more tracked parameter patterns to URL Cleaner
- [ ] Improve QR decode fallback for non-Chrome browsers
- [ ] Add dark/light theme toggle
- [ ] Add more cipher types to Text Encoder
- [ ] Improve mobile keyboard UX for Password Generator
- [ ] Add more word list entries to Passphrase Generator
- [ ] Translate UI to other languages (Bengali, Arabic, etc.)

### 🐛 Reporting Bugs

Open an [Issue](https://github.com/ocvSHANTO/privacy-forge/issues) with:
1. Which tool the bug is in
2. Steps to reproduce
3. Browser & OS you're using
4. Expected vs actual behavior

---

## 📄 License

```
MIT License

Copyright (c) 2025 Junayed Shanto

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

Full license text in [LICENSE](LICENSE).

---

## 👤 Developer

<div align="center">

<br/>

**Junayed Shanto**
*Solo Developer & Privacy Advocate · Bangladesh* 🇧🇩

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-ocvSHANTO-181717?style=for-the-badge&logo=github)](https://github.com/ocvSHANTO)
[![Instagram](https://img.shields.io/badge/Instagram-ocb__shanto-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/ocb__shanto?igsh=MXAwM3BvaTVhMXhkbA==)
[![X](https://img.shields.io/badge/X_(Twitter)-Junayed__SHANTO__-000000?style=for-the-badge&logo=x)](https://x.com/Junayed_SHANTO_)
[![YouTube](https://img.shields.io/badge/YouTube-vortexinbloom-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@vortexinbloom?si=WUHhDs4oy8OFb66y)
[![Facebook](https://img.shields.io/badge/Facebook-Junayed_Shanto-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/share/1FJzrKEALE/)

<br/>

*Built Privacy Forge to give everyone access to powerful privacy tools — free, offline, open source.*

<br/>

</div>

---

<div align="center">

**⭐ If Privacy Forge helped you, please give it a star — it helps others discover it!**

<br/>

[![Star History Chart](https://api.star-history.com/svg?repos=ocvSHANTO/privacy-forge&type=Date)](https://star-history.com/#ocvSHANTO/privacy-forge&Date)

<br/>

Made with ❤️ in Bangladesh 🇧🇩

</div>
