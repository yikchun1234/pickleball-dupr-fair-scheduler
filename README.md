<div align="center">
  <h1>🏓 Pickleball DUPR Fair Scheduler</h1>
  <p><i>A smart, AI-powered web app for generating fair Round Robin pickleball schedules based on DUPR ratings. Perfect for ReClub event organizers.</i></p>

  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" alt="License">
  
  <br>
  
  <img src="https://img.shields.io/badge/PaddleOCR-FF6F00?style=for-the-badge&logo=google_lens&logoColor=white" alt="PaddleOCR">
  <img src="https://img.shields.io/badge/ONNX_Runtime-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" alt="ONNX Runtime">
  <img src="https://img.shields.io/badge/IndexedDB-3367D6?style=for-the-badge&logo=google_chrome&logoColor=white" alt="IndexedDB">
  <img src="https://img.shields.io/badge/Cloudflare_Pages-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Cloudflare Pages">
  <img src="https://img.shields.io/badge/PWA-5A0FC8?style=for-the-badge&logo=google_chrome&logoColor=white" alt="PWA">

  <br><br>

  <img src="https://img.shields.io/github/last-commit/yikchun1234/pickleball-dupr-fair-scheduler?style=for-the-badge" alt="Last Commit">
  <img src="https://img.shields.io/github/repo-size/yikchun1234/pickleball-dupr-fair-scheduler?style=for-the-badge" alt="Repo Size">
  <img src="https://img.shields.io/badge/Live-Demo-green?style=for-the-badge" alt="Live Demo">
  
  <br><br>
  
  <a href="https://yikchun1234.github.io/pickleball-dupr-fair-scheduler/">
    <img src="https://img.shields.io/badge/_Try_Live_Demo-Click_Here-blue?style=for-the-badge" alt="Try Live Demo">
  </a>
</div>

---

### 🚀 Key Features

* **⚖️ DUPR Fair Scheduling:** Intelligent algorithm that balances DUPR ratings across courts, ensuring competitive and fair matches for every round.
* **📸 OCR Screenshot Import:** AI-powered PaddleOCR engine reads ReClub participant screenshots directly from your phone — no manual typing required.
* **🌐 100% Client-Side:** Runs entirely in your browser using ONNX Runtime WebAssembly. No server, no data upload, complete privacy.
* **📊 Advanced Statistics:** Track player rest time, DUPR variance, teammate/opponent diversity, matchup patterns, and court distribution with detailed analytics.
* **👥 Gender Balancing:** Optional gender-aware scheduling to ensure mixed-gender courts when desired.
* **📱 Mobile-First Design:** Fully responsive UI optimized for phones — add players, generate schedules, and export results on the go.
* **🌍 12 Languages:** Full interface translation in English, 中文, Bahasa Melayu, Español, Français, Tiếng Việt, ไทย, 日本語, 한국어, Deutsch, Português, and Bahasa Indonesia.
* **🌙 Dark Mode:** Full dark theme support with carefully tuned colors for schedule cards, stats report, and diff badges.
* **🎨 Theme Customization:** Pick your favorite color theme with persistent localStorage settings. Dynamic scatter triangles react to theme color.
* **💾 Export & Share:** Copy schedule to clipboard (clean `--- Round 1 ---` format) or export as formatted text for easy sharing.
* **📜 History Tracking:** Save and recall previous schedules with instant restore.
* **🎬 Smooth Animations:** Language selector and info modal popups with spring-based open/close transitions and backdrop blur.
* **ℹ️ Info Modal:** In-app introduction and feature guide accessible from the top-right (i) button.
* **📊 Matchup Pattern Analysis:** Stats summary shows per-matchup opponent and teammate repeat counts (min/avg/max).
* ** Smart Loading:** Preloads OCR engine in background with progress bar (12MB model) and rotating status messages.
* ** IndexedDB Model Cache:** OCR models cached locally after first download — instant startup on subsequent visits.
* **🏟️ Custom Court Names:** Set custom court names/numbers (e.g., "Main Court", "Side Court") based on court count dropdown.
* **🔍 Debug Mode:** Tap title 5 times to reveal raw OCR data for troubleshooting device-specific issues.
* **🔄 Auto-Refresh Stats:** Statistics panel automatically updates when regenerating schedule — no more stale data.
* **📊 Fairness Metrics:** Diff Teammate(s), Same Teammate(s), Diff Opponent(s), Same Opponent(s) columns in stats report.
* **🌐 PWA Support:** Add to Home Screen with proper pickleball paddle icon for quick mobile access.
* **🔗 Pickleball Point Counter:** Footer link to sister project for score tracking during matches.

---

### 🎯 How It Works

1. **Add Players:** Manually enter players, batch import, or upload ReClub screenshots for instant OCR detection
2. **Configure Settings:** Set target games per player, number of courts, game duration, and custom court names
3. **Generate Schedule:** Our fair algorithm distributes players across courts based on DUPR ratings
4. **Review & Export:** Check statistics, verify fairness, and share the schedule with your group

---

### 🛠️ Installation & Setup

**Option 1: Use the Live Demo (Recommended)**

Simply visit: [https://yikchun1234.github.io/pickleball-dupr-fair-scheduler/](https://yikchun1234.github.io/pickleball-dupr-fair-scheduler/)

No installation required! Works on any modern browser (Chrome, Safari, Firefox, Edge).

**Option 2: Run Locally**

**1. Clone the Repository:**

    git clone https://github.com/yikchun1234/pickleball-dupr-fair-scheduler.git
    cd pickleball-dupr-fair-scheduler

**2. Open in Browser:**

Simply open `index.html` in your web browser. That's it! No build process, no dependencies to install.

---

###  How to Use

#### Top-Right Toolbar (left to right)

| Button | Function |
|---|---|
| 🌐 Language | Open language selector (12 languages) |
| 🌙/☀️ Dark/Light | Toggle dark mode |
| ℹ️ Info | Open app introduction modal |
| 🎨 Color Picker | Choose theme color |

#### Adding Players

1. **Manual Entry:** Enter name, DUPR rating, and select gender, then click **Add**
2. **Batch Import:** Paste a list of players (one per line) in format: `Name 3.500 M`
3. **OCR Import:** Click **Upload Screenshot OCR (BETA)** and select a ReClub participant screenshot
   - 📱 Works best on ReClub app screenshots showing the "Confirmed" participant list
   - ❌ Do not use camera photos — only screenshots
   - ⚠️ OCR accuracy varies by device — please verify before importing
   - ⏳ First-time load downloads 12MB OCR models (progress bar shown); subsequent visits are instant via IndexedDB cache

#### Generating Schedule

1. Set **Target Games** per player (default: 8)
2. Set **Courts** available (auto-recommended based on player count)
3. Set **Minutes/Game** (default: 10)
4. Set **Court Names** (optional: customize court names like "Main Court", "Side Court")
5. Click **Generate Fair Schedule**

#### Viewing Statistics

Click **📊 Stats** to see:
- Games played and rest time per player
- DUPR variance per court (lower = more balanced)
- **Matchup Pattern** — opponent repeat (min/avg/max) and teammate repeat (min/max) across all matchups
- Teammate and opponent diversity metrics
- Court distribution analysis
- **Auto-refreshes** when regenerating schedule

#### Exporting Results

Click **📤 Export/Copy** to:
- Copy formatted text to clipboard (clean `--- Round 1 ---` format)
- Print or save as PDF
- Share directly with participants

---

###  Scheduling Algorithm

The fair scheduling algorithm uses a multi-factor optimization approach:

1. **DUPR Balancing:** Minimizes rating variance within each court (4 players per court)
2. **Rest Distribution:** Ensures even rest distribution across all players
3. **Gender Awareness:** Optionally balances gender ratio per court
4. **Repeat Avoidance:** Minimizes duplicate teammate/opponent pairings
5. **Court Rotation:** Rotates players across courts to ensure variety

The algorithm runs in milliseconds and produces tournament-quality schedules suitable for casual play and competitive events.

---

### 🔧 Technical Details

* **Pure Frontend:** Single HTML file with inline CSS and JavaScript
* **OCR Engine:** PaddleOCR PP-OCRv4/v5 via ONNX Runtime Web (WASM)
* **Model Caching:** IndexedDB stores 12MB OCR models locally after first download
* **No Backend:** All processing happens client-side in the browser
* **Privacy-First:** No data is sent to any server — everything stays in your browser
* **Offline Capable:** Once loaded, works without internet (except for initial model download)
* **Mobile Optimized:** Touch-friendly UI with responsive layout (breakpoint: 768px)
* **PWA Ready:** Add to Home Screen with proper icon for quick mobile access
* **Browser Support:** All modern browsers with WebAssembly support

---

### 🎨 Customization

The app supports extensive customization:

* **12 Languages:** Full UI translation with one-click switching — scroll position preserved
* **Dark Mode:** Complete dark theme with tuned colors for all components
* **Color Themes:** Choose any color for the UI (persisted in localStorage)
* **Layout:** Mobile-optimized single-row inputs and compact player list
* **Court Names:** Custom court names/numbers based on court count
* **Animated Modals:** Spring-based popup transitions with backdrop blur

**Debug Mode:** Tap the title "Pickleball DUPR" 5 times to reveal OCR debug data for troubleshooting.

---

### 📄 License & Usage

* **Non-Commercial Use:** This project is designed for personal and community pickleball events. Commercial use requires permission from the author.
* **Attribution:** If you modify or redistribute this project, please credit the original author (Amos) and link back to this repository.
* **No Warranty:** This software is provided "as-is" without warranty. Always verify generated schedules before use.

---

### 🙏 Credits & Inspiration

* **PaddleOCR:** Open-source OCR engine by Baidu
* **ONNX Runtime Web:** Cross-platform AI inference by Microsoft
* **DUPR:** Dynamic Universal Pickleball Rating system
* **ReClub:** Pickleball event management platform

---

### 🐛 Known Limitations

* **OCR Accuracy:** Varies by device screen resolution and screenshot quality. iPhone typically achieves ~100% accuracy; Android devices may require manual corrections.
* **Screenshot Format:** Currently optimized for ReClub app screenshots. Other formats may not be detected correctly.
* **Browser Memory:** Large player lists (50+) may cause memory issues on older mobile devices.

---

###  Future Enhancements

- [ ] Multi-language OCR support (Chinese player names)
- [ ] Save/load player rosters
- [ ] Tournament bracket generation
- [ ] Integration with ReClub API

---

###  Support & Feedback

Found a bug? Have a feature request? 

* Open an issue on [GitHub](https://github.com/yikchun1234/pickleball-dupr-fair-scheduler/issues)
* Connect on [ReClub](https://reclub.co/players/@amostan)

---

<div align="center">
  <b>Designed and Developed by Amos</b><br>
  <i>Making pickleball scheduling fair and fun for everyone.</i>
  <br><br>
  
  <a href="https://github.com/yikchun1234">
    <img src="https://img.shields.io/badge/GitHub-yikchun1234-181717?style=flat-square&logo=github" alt="GitHub">
  </a>
  <a href="https://reclub.co/players/@amostan">
    <img src="https://img.shields.io/badge/ReClub-@amostan-FF6B35?style=flat-square" alt="ReClub">
  </a>
  <a href="https://reclub.co/clubs/@pick-to-sync">
    <img src="https://img.shields.io/badge/Club-Pick_to_Sync-FF6B35?style=flat-square" alt="Pick to Sync">
  </a>
  <a href="https://pickleball-point-counter.cc.cd">
    <img src="https://img.shields.io/badge/Point_Counter-Sister_Project-1a5a6a?style=flat-square" alt="Pickleball Point Counter">
  </a>
</div>
