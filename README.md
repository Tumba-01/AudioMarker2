# 🎙️ AudioMarker

**AudioMarker** is a voice-driven detector/marker checklist tool built for
field use — load a numbered key, speak a number, and it gets checked off
automatically. Designed for fire alarm tests, inspection rounds, or any
scenario where your hands are busy and your voice is free.

---

## ✨ Features

### 🎤 Voice Recognition
- Speak a number and the matching entry is checked off instantly
- Supports both **English** and **German** speech recognition
- Word-to-number parsing (`"twenty one"` → `21`, `"einundzwanzig"` → `21`)
- Auto-restarts on silence — keeps listening without interaction
- Success and error audio feedback via Web Audio API
- Haptic vibration feedback on mobile

### 📋 Checklist
- Load a numbered key via `.txt` or `.json` file
- Add place/location notes per entry
- Manual checkbox override at any time
- Reset all checkboxes in one tap
- Random 50% auto-check for test/demo purposes
- Smooth auto-scroll to newly checked rows

### 📊 Progress Tracking
- Live `checked / total` counter
- Animated progress bar — turns gold when 100% complete

### 💾 Import / Export
- Export as **JSON** (full session data, importable later)
- Export as **PDF** (formatted report via jsPDF, A4, paginated)
- Import a previous session — restores checked state, places & comments
- Unchecked entries require a comment/reason before export

### 🌍 Bilingual
- Full **English** and **German** UI with one-tap toggle
- Language persists across sessions and is saved in exports

### 📱 Mobile Ready
- Wake Lock API — keeps screen on during active recording
- Responsive layout
- Touch-friendly controls

### 🎨 Theme System
22 themes across retro, OS, and gaming categories — all persistent via
`localStorage` and selectable from the slide-in theme drawer.

---

## 🎨 Themes

| Category | Themes |
|---|---|
| **Dark UI** | Obsidian Glow, Neural Pulse, Amethyst, Solar Flare, Console, Kinetic, Stellar, Sovereign, Nocturne |
| **OS / Retro** | Windows 96, Windows XP, Metro Dark, MS-DOS, Mac OS 1 (1984), Commodore 64 |
| **Mobile OS** | One UI (Samsung), iOS 18 (Apple) |
| **Gaming** | Hazmat ☢️, Cyberpunk 2077 ⚡, NFS Most Wanted 🚗, CS:GO 🔫 |
| **Special** | Chroma ✨ |

---

## 🚀 Getting Started

No build step required — pure HTML, CSS and JavaScript.

```bash
git clone https://github.com/yourname/audiomarker.git
cd audiomarker
# open index.html in your browser
