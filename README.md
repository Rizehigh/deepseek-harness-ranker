# DeepSeek Harness GitHub Ranker 🚀

> A sleek, high-performance **Material 3** web dashboard to discover, rank, and track top GitHub repositories related to **DeepSeek Harness**.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![GitHub Pages](https://img.shields.io/badge/deployment-GitHub%20Pages-success.svg)
![Build](https://img.shields.io/badge/dependencies-zero-brightgreen.svg)

---

## ✨ Features

- 🏆 **Top 3 Podium**: Highlighted podium cards for top 3 repositories with medal badges and rank styling.
- 🚀 **Automated Growth Tracking (`+N` Deltas)**: Tracks daily/weekly growth in Stars, Forks, and Open Issues using automated GitHub Action snapshots (`data/history.json`).
- 🎯 **Category Filter Chips**: Filter projects on the fly:
  - **All Repositories**
  - **Agents & Swarms**
  - **Harness & SDKs**
  - **Evals & Benchmarks**
  - **Emerging (<1k Stars)**
- ⚡ **Instant Inline SVG Rendering**: Zero external font dependencies (0ms render-blocking load time).
- 🎨 **Material 3 Dark System**: Designed with M3 dark tokens, elevated surface cards, state layers, and typography (`Plus Jakarta Sans` + `JetBrains Mono`).
- ⚡ **Performance & Caching**: Client-side `sessionStorage` caching (5-min TTL) and `localStorage` token persistence to mitigate API rate limits.
- 🆕 **Dynamic "New" Project Detection**: Automatically badges projects created within the selected period.

---

## 🛠️ Tech Stack

- **Frontend**: Plain HTML5, CSS3 (Material 3 Tokens), Vanilla JS (ES6+).
- **Icons**: Inline SVGs (No external web fonts).
- **Typography**: Google Fonts (*Plus Jakarta Sans*, *JetBrains Mono*).
- **API**: GitHub REST Search API (`/search/repositories`).
- **Automation**: GitHub Actions (`.github/workflows/snapshot.yml`).

---

## 📁 Repository Structure

```
deepseek-harness-github-ranker/
├── .github/
│   └── workflows/
│       └── snapshot.yml     # Automated daily stat recorder (Runs 00:00 UTC)
├── data/
│   └── history.json         # Historical daily repository snapshots
├── index.html               # Main single-page web app
└── README.md                # Project documentation
```

---

## 🚀 GitHub Pages Deployment Guide

Deploying this app is 100% free with **zero build steps**:

### 1. Push Code to GitHub
```bash
git add .
git commit -m "feat: initial release"
git push origin main
```

### 2. Enable GitHub Pages
1. Go to your repository on **GitHub.com**.
2. Navigate to **Settings** > **Pages** (under Code and automation).
3. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`.
   - **Branch**: Choose `main` branch and `/ (root)` folder.
4. Click **Save**.
5. Your site will be live at: `https://<your-username>.github.io/<repo-name>/`

### 3. Enable Automated Daily Snapshots
1. On GitHub, go to the **Actions** tab.
2. Select **"Daily Repository Stats Snapshot"**.
3. Click **Run workflow** > **Run workflow** to generate your first snapshot!

---

## 💻 Local Development

No build tool (npm, vite, etc.) is required. To run locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/deepseek-harness-github-ranker.git
   cd deepseek-harness-github-ranker
   ```

2. Open `index.html` directly in any web browser, or serve it using Python:
   ```bash
   python3 -m http.server 8000
   ```
3. Visit `http://localhost:8000` in your browser.

---

## 📄 License

Distributed under the **MIT License**.
