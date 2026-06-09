# 🔪 NEXUS — The Text & QR Multitool

A futuristic, **100% offline**, single-file web app. No build steps, no accounts, no tracking, no internet required. Just open the HTML file (or host it anywhere) and everything works.

> A digital Swiss Army knife for text, encodings, hashes, QR codes & more.

---

## ✨ Features

### ⇄ Converter
Convert text between **31 reversible encodings**, with a searchable dropdown.
- **Number bases:** Binary, Octal, Decimal, Hexadecimal (+ spaced hex)
- **Binary→Text:** Base32, Base32hex, Base45, Base58, Base62, Base64, Base64URL, Ascii85, Z85, Uuencode, Xxencode
- **Web:** URL/Percent, HTML entities, HTML numeric, Quoted-Printable, Unicode code points, JS escapes
- **Ciphers:** ROT13, ROT47, ROT5, Atbash, Morse, NATO phonetic, Leetspeak, Reversed
- 🔍 **Auto-detect** the input encoding · 🧮 live char/word/byte/line stats · 💾 history · 📋 copy as data-URI

### 🔢 Hash
Live digests as you type: **SHA-1, SHA-256, SHA-384, SHA-512, MD5, CRC32**. Click any to copy.

### 🎲 Generators
- **UUID v4** (single or ×5)
- **Password generator** with length slider, character-set toggles, "no ambiguous" option & entropy strength meter
- **Random bytes** (hex) — useful for keys, tokens, salts

### ▣ QR Scanner
Scan via **webcam** or **image upload / drag-and-drop**. Decodes QR codes (and barcodes where the browser supports `BarcodeDetector`) and shows the data as **raw text, hex, Base64, binary, decimal bytes**, plus auto type-detection (URL, WiFi, vCard, 2FA, etc.).

### ⊞ QR Generator
Make **branded, scannable QR codes** — better than the online tools:
- 🎨 Style presets: YouTube, WhatsApp, Instagram, TikTok, Spotify, Facebook, X, LinkedIn, Email, WiFi
- 📣 Call-to-action label bar (e.g. *"Watch Now!"*)
- 🎨 Custom colors · 🔵 dot/rounded/square shapes · 🌈 gradient dots
- 📤 Upload your own center logo
- 🔗 Auto-adds `https://` to links
- ⬇ Download as **PNG** or 🖨 **SVG** (filename = your content)

### 🎡 Wheel
A spinning wheel of names with **sound effects, ticking, confetti, a winner popup & history**. Includes shuffle / sort / clear and a "remove winner after spin" mode.

### 🎬 Video
Load your own video (stays on your device) and:
- 🎬 **Make GIF** — animated GIF with adjustable fps & width (built-in encoder, no libraries)
- ✂️ **Trim → WebM** — cut a clip and download it
- 🔇 **Extract Audio** — pull the audio out as a lossless WAV
- 🖼️ **Grab Frames** — capture screenshots from the clip
- Trim sliders, live preview & progress bar

### 🗜️ Image
Compress & resize images locally — max-width and quality sliders, output as **JPEG / WebP / PNG**, shows how much you saved.

### 🎨 ASCII Art
Turn any image into **colored ASCII art**. Multiple character sets, width control, invert option. Export as plain text, **ANSI color codes** (paste into a terminal!) or a **PNG**.

### 📹 Recorder
Record your **screen / window / tab** with optional microphone and system audio. Live timer, preview, and download as WebM.

---

## 🚀 Usage

**Option 1 — Just open it**
Download `converter.html` (or `index.html`) and double-click it. Works fully offline, including the camera & QR features.

**Option 2 — Host on GitHub Pages (free)**
1. Create a new **public** repository and upload `index.html`.
2. Go to **Settings → Pages**.
3. Under *Branch*, pick **main** and **/(root)**, then **Save**.
4. Your site goes live at: [https://YOUR-USERNAME.github.io/REPO-NAME/](https://YOUR-USERNAME.github.io/REPO-NAME/)
---

## ⌨️ Keyboard Shortcuts
| Shortcut | Action |
|---|---|
| `Ctrl/Cmd + 1–9` | Switch tabs |
| `Ctrl/Cmd + Enter` | Convert / Generate |
| `Ctrl/Cmd + Shift + C` | Copy output |

---

## 🔒 Privacy
Everything runs **locally in your browser**. Nothing is uploaded, nothing is tracked, and the file has **zero external dependencies** — the QR libraries are bundled inside.

---

## 🛠️ Tech
- Single self-contained `index.html` (HTML + CSS + JS)
- [jsQR](https://github.com/cozmo/jsQR) — QR scanning, inlined
- [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) — QR generation, inlined
- WebCrypto for SHA hashes; pure-JS MD5 & CRC32

---

© 2026 TheCookieGod64.
Licensed under the **Apache License 2.0** — see [`LICENSE`](LICENSE) and [`NOTICE`](NOTICE).
Built with way too much fire 🔥🔪
