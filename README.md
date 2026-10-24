# 🏺 Ayo Daily — African Mancala Strategy Game

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PWA Ready](https://img.shields.io/badge/PWA-Ready-green.svg)](https://jamesabaa.github.io/ayo-daily/)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-0-blue.svg)](https://jamesabaa.github.io/ayo-daily/)

**Live Game:** [https://jamesabaa.github.io/ayo-daily/](https://jamesabaa.github.io/ayo-daily/)

Ayo Daily is a modern, responsive, privacy-friendly implementation of **Ayo Olopon / Oware**—one of the oldest mathematical strategy board games in the world, originating from the Yoruba culture of West Africa.

---

## ✨ Features & Upgrades

- 🗓️ **Daily Challenge:** Synchronized globally by date (UTC). Every player gets the exact same mystery opening board.
- 🏺 **Classic Mode:** Standard 4-seeds-per-pit tournament Oware match.
- 🧠 **Minimax AI Engine:** 3 selectable difficulty levels:
  - **Casual:** Fast & friendly for learning.
  - **Clever:** Tactical depth 2 search with feeding awareness.
  - **Master:** High-level search maximizing captures, seed safety, and board mobility.
- 🔊 **Zero-Asset Web Audio:** Organic wooden clicks, capture harmonics, win fanfare, and defeat cadences synthesised live in the browser without loading any MP3 files.
- 💫 **Animated Sowing & Visual Trails:** Watch seeds drop pit-by-pit with highlight trails and gold flashes on capture.
- ↩️ **Undo Move:** Made a mistake? Undo your last move in Classic mode.
- 📊 **Streaks & Statistics:** Tracks games played, win rate %, current streak, max streak, and total captured seeds in `localStorage`.
- 📤 **Wordle-Style Viral Sharing:** One-click share with emoji scorecards (`navigator.share` or clipboard copy).
- 💰 **Google AdSense Ready:** Pre-configured banner slots, result interstitial slots, GDPR/CCPA cookie consent banner, and mandatory policy pages (Privacy Policy, Terms of Service, About History).
- 📱 **PWA & Offline Capable:** Installable to mobile and desktop home screens with service worker offline caching.

---

## 💰 How to Connect Google AdSense & Monetize

### 1. Replace the Placeholder Publisher ID
In `index.html`:
1. Find `ca-pub-XXXXXXXXXXXXXXXX` in the `<head>` script tag:
   ```html
   <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR_ID_HERE" crossorigin="anonymous"></script>
   ```
2. Replace `ca-pub-XXXXXXXXXXXXXXXX` in the top ad slot and result ad slot with your ad slot IDs.
3. Update `AYO_CONFIG.adsenseClient` inside the script block.

### 2. Update `ads.txt`
Open `ads.txt` and replace:
```
google.com, pub-XXXXXXXXXXXXXXXX, DIRECT, f08c47fec0942fa0
```
with your actual publisher ID number (e.g. `pub-1234567890123456`).

### 3. Crucial Tips for Getting AdSense Approval
Google AdSense frequently rejects simple single-page games for **"Low Value Content"**. Ayo Daily is now equipped with:
- Dedicated **About Ayo History & Culture** section explaining the Yoruba origins and mathematics of Mancala.
- Detailed **Privacy Policy** complying with Google's cookie and DART policies.
- Full **Terms of Use**.
- **Cookie Consent Banner** for EU/GDPR compliance.

> **Pro-Tip:** Google AdSense approvals are significantly higher with a custom domain (e.g., `ayodaily.com` or `playayo.com`) rather than a default `github.io` subdomain.

---

## 🚀 How to Make It Live on GitHub Pages

1. **Commit and Push Your Changes:**
   ```bash
   git add .
   git commit -m "Upgrade Ayo Daily: sound, stats, PWA, share, and AdSense readiness"
   git push origin main
   ```
2. **Verify GitHub Pages:**
   - Go to your repository settings on GitHub: `https://github.com/Jamesabaa/ayo-daily/settings/pages`
   - Source: **Deploy from a branch**
   - Branch: **`main`** / `/ (root)`
   - Click **Save**.
   - Your site will update in 1–2 minutes at `https://jamesabaa.github.io/ayo-daily/`.

---

## 🌐 Connecting a Custom Domain (Optional & Recommended)

1. Purchase a domain from Namecheap, Porkbun, or GoDaddy (e.g., `ayodaily.com`).
2. In your GitHub repository **Settings -> Pages -> Custom domain**, enter your domain name.
3. In your DNS provider, create:
   - **Apex domain (A Records):**
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - **www subdomain (CNAME Record):**
     - `www` -> `jamesabaa.github.io`
4. Check **Enforce HTTPS** in GitHub Pages.
