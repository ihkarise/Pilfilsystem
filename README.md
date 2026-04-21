<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/896b30ab-06f0-4495-ac68-bc787baa43e3

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

## Deploy to GitHub Pages (Project Repo)

This app uses `HashRouter`, so routes work on GitHub Pages without server rewrites.

1. Ensure your repository has GitHub Pages configured to **GitHub Actions**.
2. Keep `VITE_BASE_PATH` aligned to your repo path (for this repo: `/Pilfilsystem/`).
3. Push to `main` (or run the `Deploy static content to Pages` workflow manually).
4. Open:
   `https://<your-github-username>.github.io/Pilfilsystem/`

If you still see a blank page, open browser dev tools and confirm:
- JS/CSS are loading from `/Pilfilsystem/assets/...` (not from `/assets/...`).
- Images are loading from `/Pilfilsystem/...` (not from `/...`).
