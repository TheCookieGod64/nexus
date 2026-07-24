# 🔪 NEXUS — The Single-File Multitool Workstation

A futuristic, **100% offline**, single-file web app. No build steps, no accounts, no tracking, no internet required. Just open the HTML file (or host it anywhere) and everything works.

> A digital Swiss Army knife for text, encodings, hashes, QR codes, media tools, network utilities & more — now reorganized into cohesive **Unified Workstations**.

---

## ✨ The 7 Main Workstations

### 1. ⇄ Data & Files
- **Converter:** Convert text between **31 reversible encodings** (Binary, Base32/45/58/62/64, Z85, ROT ciphers, Morse, Leetspeak) with auto-detection and live stats.
- **Code Formatter:** Pretty-print and minify JSON, XML, SQL, and CSS.
- **File Codec (Jailbreak):** Turn **any binary file** (images, videos, executables) into a portable text/Base64/Hex representation, or decode it back to its original raw format.

### 2. 🔒 Crypto & Auth
- **Hashes:** Live digests as you type for **SHA-1, SHA-256, SHA-384, SHA-512, MD5, CRC32**.
- **Generators:** Secure UUID v4 generator, Password Generator with custom character sets and length sliders, and Random Hex Bytes.
- **Entropy Meter:** Live password security score, entropy strength calculations, and security checklist.
- **JWT Inspector:** Decode, inspect, and verify JSON Web Tokens on the fly.

### 3. ▣ QR Studio
- **Scanner & Decoder:** Scan QR codes and barcodes via **webcam** or image drag-and-drop. View decoded data in raw text, hex, Base64, binary, or decimal bytes. Auto-detects URLs, WiFi, vCards, 2FA OTPs, etc.
- **Custom QR Generator:** Make beautiful branded QR codes with custom styling presets (YouTube, Spotify, WhatsApp, Wi-Fi), call-to-action labels, custom colors, gradient dots, and central logo uploads. Export as PNG or SVG.

### 4. 🖼️ Visual & Media
- **Video Studio:** Completely local video processing. Build animated GIFs, trim video clips to WebM, extract audio to lossless WAV, or grab exact frame screenshots.
- **Image Compressor:** Resize and compress JPEG/WebP/PNG images locally.
- **Base64 Image:** Live two-way converter between Base64 strings and image previews.
- **ASCII Art Generator:** Convert any uploaded image into colored ASCII / ANSI text art or standalone PNGs.
- **Color Palette:** Spacebar-driven harmony generator with instant CSS exports.
- **Screen Recorder:** Capture your screen, window, or tab (with optional microphone/system audio) directly to WebM.

### 5. 🌐 Net & Dev
- **REST API Client:** A mini-Postman HTTP requester for testing endpoints directly.
- **Subnet Calculator:** IP and CIDR subnet calculator showing network ranges, broadcast addresses, and wildcard masks.

### 6. ⚡ Time & Tools
- **Pomodoro Focus Timer & Stopwatch:** Features an **unthrottled Web Worker Master Clock** and wall-clock timestamps. Timers keep running accurately in the background even when your browser tab is inactive or hidden. Alerts via sound and web notifications.
- **Epoch Time:** Convert Unix timestamps to human-readable local dates and vice versa.
- **Markdown Live Editor:** Side-by-side live Markdown rendering and editor.
- **Wheel of Names:** Ticking spinning wheel with sound effects, victory confetti, winner popups, and exclusion modes.

### 7. 🕹️ RetroArch
- **Browser Emulator:** RetroArch in your browser — powered by [EmulatorJS](https://emulatorjs.org) running **libretro cores compiled to WebAssembly**. Import any ROM you own (drag-and-drop or file picker) and play instantly.
- **30+ Systems:** NES, SNES, Game Boy / Color / Advance, Nintendo DS & 64, Virtual Boy, Sega Genesis / Master System / Game Gear / CD / Saturn, PC Engine / TurboGrafx-16, PlayStation, Atari 2600 / 7800 / Lynx, Neo Geo Pocket, WonderSwan, ColecoVision, and Arcade (FBNeo / MAME).
- **Smart Auto-Detect:** Picks the correct core from your file's extension (`.nes`, `.sfc`, `.gba`, `.z64`, `.chd`, `.zip`, …) with a manual override dropdown.
- **🔗 Joy-Con Auto-Combine:** Pair a left **and** right Nintendo Switch Joy-Con over Bluetooth and NEXUS **automatically fuses them into a single controller** (it transparently merges the browser's two separate gamepads into one standard pad). No more fiddly manual pairing — toggleable, with a live controller-detection status strip and optional debug readout.
- **⛶ One-Tap Fullscreen:** A dedicated fullscreen button for distraction-free play.
- **📱 Mobile Touch Controls:** On phones/tablets, **transparent on-screen controls** (D-pad, A/B/X/Y, L/R shoulders, Start/Select) appear automatically in fullscreen. Multi-touch ready and toggleable.
- **Full Emulator Features:** On-screen menu for save states, load states, and fast-forward. Physical USB/Bluetooth gamepads and keyboard controls work out of the box.

> 🔌 **Note:** Unlike the rest of NEXUS, the RetroArch tab streams emulator cores from `cdn.emulatorjs.org` on first boot of each system (cached afterward). **Your ROM files never leave your device** — all emulation runs 100% locally in WASM.

---

## 🚀 Usage

**Option 1 — Just open it**
Download `index.html` and double-click it. Works fully offline, including the webcam, QR tools, and video encoding.

**Option 2 — Host on GitHub Pages (free)**
1. Create a new **public** repository and upload `index.html`.
2. Go to **Settings → Pages**.
3. Under *Branch*, pick **main** and **/(root)**, then **Save**.
4. Your site goes live at: `https://YOUR-USERNAME.github.io/REPO-NAME/`

---

## ⌨️ Keyboard Shortcuts
| Shortcut | Action |
|---|---|
| `Ctrl/Cmd + 1–7` | Switch Main Workstations |
| `Alt/Option + 1–9` | Filter sub-tools within the active workstation |
| `Ctrl/Cmd + Enter` | Convert / Generate / Run |
| `Ctrl/Cmd + Shift + C` | Copy primary output |
| `Space` | Generate new color palette (when Palette tool is visible) |

---

## 🔒 Privacy & Architecture
Everything runs **locally in your browser**. Nothing is uploaded, nothing is tracked, and the file has **zero external dependencies** — the scanning and generation libraries are fully inlined inside `index.html`.

Background timers (Pomodoro & Stopwatch) utilize an advanced inline Web Worker architecture, completely bypassing browser background-tab throttling.

---

© 2026 TheCookieGod64.
Licensed under the **Apache License 2.0** — see [`LICENSE`](LICENSE) and [`NOTICE`](NOTICE).
Built with way too much fire 🔥🔪
