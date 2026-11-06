# Casawi Running — Urban Streetwear Storefront

Casablanca urban streetwear & athletic drops storefront with trilingual support (Français, العربية, English), Moroccan Dirham (MAD) pricing, interactive cart, Moroccan courier checkout, and automated WhatsApp order dispatch to **+212 694-940173** and TikTok **@casawirunning1**.

---

## 🚀 How to Publish to GitHub Pages

Modern web apps written in React, TypeScript, and Tailwind need to be bundled into static HTML, CSS, and JS before browsers can run them. This repository gives you **3 easy ways** to publish to GitHub Pages:

---

### Option A: The Recommended Way (Automated GitHub Actions — 1 Minute)

This repository includes a pre-configured GitHub Actions workflow in `.github/workflows/deploy.yml`.

1. Push this repository to GitHub:
   ```bash
   git add .
   git commit -m "Launch Casawi Running"
   git push origin main
   ```
2. On GitHub, navigate to your repository:
   - Go to **Settings** → **Pages** (in the left sidebar).
   - Under **Build and deployment** → **Source**, select **GitHub Actions**.
3. That's it! GitHub will automatically compile the code and host your site live at `https://<your-username>.github.io/<your-repo-name>/`.

---

### Option B: Direct 1-Click from `/docs` Folder (No Node.js Required)

If you prefer GitHub Pages to serve static files from a specific folder:

1. We have pre-compiled the static assets directly into the `/docs` folder:
   ```
   docs/
   ├── index.html
   └── assets/
       ├── index-*.css
       └── index-*.js
   ```
2. In your repository on GitHub:
   - Go to **Settings** → **Pages**.
   - Under **Source**, select **Deploy from a branch**.
   - Set **Branch** to `main` (or `master`) and select folder **/docs**.
   - Click **Save**.
3. Your site is live immediately!

---

### Option C: Instant Terminal Command (`npm run deploy`)

You can publish the production build directly to a dedicated `gh-pages` branch:

```bash
npm install
npm run deploy
```

This builds the project and pushes the static bundle directly to the `gh-pages` branch on your GitHub repository.

---

### Option D: Plain Root Structure (`index.html` at repository root)

If you strictly want your repository root to have only `index.html` and compiled assets:

1. Run `npm run build`.
2. Move the files inside `dist/` to your root directory:
   ```
   your-repository/
   ├── index.html
   ├── assets/
   │   ├── index.css
   │   └── index.js
   └── README.md
   ```
3. In GitHub Settings → Pages, select **Branch: main** and **Folder: / (root)**.

---

## 🛠️ Project Configuration

- **Vite Base Path**: Configured as `base: './'` in `vite.config.ts` so relative asset paths work anywhere (custom domains, GitHub Pages subpaths, or local files).
- **Store WhatsApp**: `+212 694-940173`
- **TikTok Community**: `@casawirunning1`
- **Currency**: Moroccan Dirham (MAD / د.م.)
- **Payment Method**: Cash on Delivery (*Paiement à la livraison / الدفع عند الاستلام*)

---

## 💻 Local Development

```bash
# 1. Install dependencies
npm install

# 2. Run local development server
npm run dev

# 3. Build static distribution
npm run build
```
