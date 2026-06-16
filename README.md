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
  <img src="https://img.shields.io/badge/Cloudflare_Pages-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Cloudflare Pages">

  <br><br>

  <img src="https://img.shields.io/github/last-commit/yikchun1234/pickleball-dupr-fair-scheduler?style=for-the-badge" alt="Last Commit">
  <img src="https://img.shields.io/github/repo-size/yikchun1234/pickleball-dupr-fair-scheduler?style=for-the-badge" alt="Repo Size">
  <img src="https://img.shields.io/badge/Live-Demo-green?style=for-the-badge" alt="Live Demo">
  
  <br><br>
  
  <a href="https://pb-fair-games.pages.dev">
    <img src="https://img.shields.io/badge/🚀_Try_Live_Demo-Click_Here-blue?style=for-the-badge" alt="Try Live Demo">
  </a>
</div>

---

### 🚀 Key Features

* **⚖️ DUPR Fair Scheduling:** Intelligent algorithm that balances DUPR ratings across courts, ensuring competitive and fair matches for every round.
* **📸 OCR Screenshot Import:** AI-powered PaddleOCR engine reads ReClub participant screenshots directly from your phone — no manual typing required.
* **🌐 100% Client-Side:** Runs entirely in your browser using ONNX Runtime WebAssembly. No server, no data upload, complete privacy.
* **📊 Advanced Statistics:** Track player rest time, DUPR variance, teammate/opponent diversity, and court distribution with detailed analytics.
* **👥 Gender Balancing:** Optional gender-aware scheduling to ensure mixed-gender courts when desired.
* **📱 Mobile-First Design:** Fully responsive UI optimized for phones — add players, generate schedules, and export results on the go.
* **🎨 Theme Customization:** Pick your favorite color theme with persistent localStorage settings.
* **🌍 Bilingual Support:** Full English and 中文 (Chinese) interface with one-click language switching.
* **💾 Export & Share:** Copy schedule to clipboard or export as formatted text for easy sharing with participants.
* **📜 History Tracking:** Save and recall previous schedules with instant restore.
* **⚡ Smart Loading:** Preloads OCR engine in background with loading indicator — no more waiting when you need to scan.
* **🔍 Debug Mode:** Tap title 5 times to reveal raw OCR data for troubleshooting device-specific issues.

---

### 🎯 How It Works

1. **Add Players:** Manually enter players or upload ReClub screenshots for instant OCR detection
2. **Configure Settings:** Set target games per player, number of courts, and minimum games per round
3. **Generate Schedule:** Our fair algorithm distributes players across courts based on DUPR ratings
4. **Review & Export:** Check statistics, verify fairness, and share the schedule with your group

---

### 🛠️ Installation & Setup

**Option 1: Use the Live Demo (Recommended)**

Simply visit: [https://pb-fair-games.pages.dev](https://pb-fair-games.pages.dev)

No installation required! Works on any modern browser (Chrome, Safari, Firefox, Edge).

**Option 2: Run Locally**

**1. Clone the Repository:**

    git clone https://github.com/yikchun1234/pickleball-dupr-fair-scheduler.git
    cd pickleball-dupr-fair-scheduler

**2. Open in Browser:**

Simply open `index.html` in your web browser. That's it! No build process, no dependencies to install.

---

### 📱 How to Use

#### Adding Players

1. **Manual Entry:** Enter name, DUPR rating, and select gender, then click **Add**
2. **Batch Import:** Paste a list of players (one per line) in format: `Name 3.500`
3. **OCR Import:** Click **Upload Screenshot OCR (BETA)** and select a ReClub participant screenshot
   - 📱 Works best on ReClub app screenshots showing the "Confirmed" participant list
   - ❌ Do not use camera photos — only screenshots
   - ⚠️ OCR accuracy varies by device — please verify before importing

#### Generating Schedule

1. Set **Target Games** per player (default: 8)
2. Set **Courts** available (auto-recommended based on player count)
3. Set **Min Games/Round** (default: 1)
4. Click **Generate Fair Schedule**

#### Viewing Statistics

Click **📊 View Statistics** to see:
- Games played and rest time per player
- DUPR variance per court (lower = more balanced)
- Teammate and opponent diversity metrics
- Court distribution analysis

#### Exporting Results

Click **📤 Export Schedule** to:
- Copy formatted text to clipboard
- Print or save as PDF
- Share directly with participants

---

### 🧮 Scheduling Algorithm

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
* **No Backend:** All processing happens client-side in the browser
* **Privacy-First:** No data is sent to any server — everything stays in your browser
* **Offline Capable:** Once loaded, works without internet (except for initial model download)
* **Mobile Optimized:** Touch-friendly UI with responsive layout (breakpoint: 768px)
* **Browser Support:** All modern browsers with WebAssembly support

---

### 🎨 Customization

The app supports extensive customization via the theme picker:

* **Color Themes:** Choose any color for the UI (persisted in localStorage)
* **Language:** Toggle between English and Chinese
* **Layout:** Mobile-optimized single-row inputs and compact player list

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

### 🔮 Future Enhancements

- [ ] Multi-language OCR support (Chinese player names)
- [ ] Save/load player rosters
- [ ] Tournament bracket generation
- [ ] Integration with ReClub API
- [ ] Offline PWA (Progressive Web App) support

---

### 📞 Support & Feedback

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
</div>
