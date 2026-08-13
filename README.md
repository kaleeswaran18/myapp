# சொல் களஞ்சியம் (Word Treasury) — Tamil-English Vocabulary App

## Run locally

1. Install [Node.js](https://nodejs.org) (v18+) if you don't have it.
2. Open a terminal in this folder and run:

```bash
npm install
npm run dev
```

3. Open the URL it shows (usually `http://localhost:5173`) in your browser.

The 🔊 speaker buttons use your browser's built-in text-to-speech
(`speechSynthesis`), which works normally in a real browser — it only
fails inside the Claude preview sandbox. Progress (learned words) is
saved in your browser's `localStorage`, so it stays even after you
close and reopen the tab.

## Build for deployment

```bash
npm run build
```

This creates a `dist/` folder you can upload to any static host
(Vercel, Netlify, GitHub Pages, etc.) or bundle into a React Native /
mobile shell later.

## Notes

- Tamil voice quality depends on the voices installed on the device/
  browser. Chrome and Edge on Windows/Android generally have a decent
  `ta-IN` voice; if a device has none, it falls back to a default
  voice.
- All 390 words are bundled directly in `src/App.jsx` — no external
  API calls needed for the word data itself.
