# DeepSeek Harness GitHub Ranker

A fast, responsive Material 3 web application to discover and rank top GitHub repositories related to **DeepSeek Harness**.

## Features

- 🏆 **Podium Display**: Displays the top 3 repositories on a podium layout with distinct gold, silver, and bronze rank accents.
- 📊 **Multiple Metrics**: Filter rankings by **Stars**, **Forks**, or **Watchers**.
- ⏱️ **Flexible Timeframes**: Discover trending repositories over the past **day**, **week**, **month**, or **year**.
- 🔢 **Customizable Top N**: Toggle between Top 20, Top 50, or Top 100 repositories.
- ⚡ **Rate Limit & Performance Optimization**:
  - Automatic `sessionStorage` caching (5-minute TTL) to prevent duplicate API requests.
  - Live API rate limit counter.
  - Optional personal GitHub access token support for higher request limits.
  - Auto-retrying rate limit indicator.
- 🔍 **Instant Search Bar**: Filter loaded repositories by name, description, or owner in real-time.
- 🎨 **Material 3 Dark Theme**: Designed using Google's Material 3 design tokens, typography (Plus Jakarta Sans & JetBrains Mono), and icons.

## Quick Start (Local)

Simply open `index.html` in any web browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then navigate to `http://localhost:8000`.

## Deploying to GitHub Pages

1. Push this repository to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git branch -M main
   git push -u origin main
   ```
2. In your GitHub repository, go to **Settings** > **Pages**.
3. Under **Build and deployment** > **Source**, select **Deploy from a branch**.
4. Choose the **main** branch and **/** (root) folder, then click **Save**.
5. Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/` in a couple of minutes!

## License

MIT
