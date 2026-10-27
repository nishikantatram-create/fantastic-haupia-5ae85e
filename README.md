# Verbos — Offline Spanish Verb Conjugation & Pronunciation App

**Verbos** is a lightweight, mobile-first Progressive Web App (PWA) designed for Spanish language learners. It offers complete tense conjugations across CEFR levels (A1–B1), full usage notes, contextual example sentences, and offline native Spanish text-to-speech pronunciation.

🔗 **Live Demo:** [https://fantastic-haupia-5ae85e.netlify.app](https://fantastic-haupia-5ae85e.netlify.app)

---

## Features

- **Categorized by Proficiency & Tense:** Explore verbs categorized across CEFR levels (**A1**, **A2**, **B1**) and key tenses (Presente, Pretérito Perfecto, Pretérito Indefinido, Imperfecto, Futuro Simple, Condicional, Subjuntivo, Imperativo, and more).
- **Audio Pronunciation:** Tap any conjugation card to hear native Spanish pronunciation powered by the Web Speech API (`SpeechSynthesis`). Includes an adjustable playback speed slider.
- **100% Offline Capable (PWA):** Built with Service Workers to cache all application shell files and datasets locally. Operates reliably without an active internet connection.
- **Installable Native Experience:** Can be installed directly to home screens on Android, iOS, Windows, and macOS with zero app-store overhead.
- **Fast & Dependency-Free:** Developed in clean vanilla JavaScript, HTML5, and modern CSS with custom dark mode and responsive layouts.

---

## File Structure

```text
├── index.html        # App UI, routing, state management, and Web Speech engine
├── data.js           # Spanish verbs dataset (conjugations, sentences, translations)
├── manifest.json     # PWA manifest (app metadata, theme color, icons)
├── sw.js             # Service Worker for local caching and offline functionality
├── icon-192.png      # 192x192 app icon
├── icon-512.png      # 512x512 app icon
└── README.md         # Project documentation
```

---

## How to Install on Mobile

### Android (Chrome)
1. Open [https://fantastic-haupia-5ae85e.netlify.app](https://fantastic-haupia-5ae85e.netlify.app) in Google Chrome.
2. Tap the three dots menu (**⋮**) in the top right corner.
3. Select **Install app** (or **Add to Home screen**).
4. Tap **Install** to add the standalone app to your app drawer and home screen.

### iOS (Safari)
1. Open [https://fantastic-haupia-5ae85e.netlify.app](https://fantastic-haupia-5ae85e.netlify.app) in Safari.
2. Tap the **Share** button (box with an upward arrow) at the bottom.
3. Scroll down and select **Add to Home Screen**.
4. Tap **Add**.

---

## Local Development

No package managers or build steps are required.

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/verbos.git
   cd verbos
   ```
2. Run a local development server:
   ```bash
   python -m http.server 8000
   ```
3. Open `http://localhost:8000` in your browser.

> **Note:** The Web Speech API and Service Workers require a secure context (`https://` or `localhost`) to operate properly.

---

## Tech Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript (ES6+)
- **Audio Engine:** Web Speech API (`window.speechSynthesis`)
- **PWA Architecture:** Service Workers & Web App Manifest
- **Hosting:** Netlify / GitHub Pages

---

## License

MIT License. Free to use and adapt for language study and educational projects.
