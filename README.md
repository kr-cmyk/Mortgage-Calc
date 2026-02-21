# Mortgage Calculator PWA

A commercial mortgage calculator that installs directly to your iPhone home screen.

## Features
- NCF/NOI, Loan Amount, Rate, Term, Amortization, Day Count Convention (30/360 & ACT/360)
- Loan Constant (K), DSCR, Debt Yield, Maturity Balance
- Toggle between annual summary and full monthly amortization schedule
- Save unlimited named scenarios
- Side-by-side scenario comparison with best-value highlighting
- Works fully offline once installed

---

## How to Install on iPhone (2 steps)

### Step 1 — Host on GitHub Pages (free, ~5 minutes)

1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click **+** → **New repository**
3. Name it `mortgage-calc` (or anything you like)
4. Set it to **Public**, click **Create repository**
5. Click **uploading an existing file**
6. Drag all 5 files into the upload area:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
7. Click **Commit changes**
8. Go to **Settings** → **Pages**
9. Under "Source" select **Deploy from a branch** → **main** → **/ (root)**
10. Click **Save**
11. After ~1 minute, your URL will be: `https://YOUR-USERNAME.github.io/mortgage-calc/`

### Step 2 — Add to iPhone Home Screen

1. Open Safari on your iPhone (must be Safari, not Chrome)
2. Go to your GitHub Pages URL from Step 1
3. Tap the **Share** button (box with arrow pointing up)
4. Scroll down and tap **"Add to Home Screen"**
5. Tap **Add**

The app now appears on your home screen like a native app — full screen, no browser chrome, works offline.

---

## Files
| File | Purpose |
|------|---------|
| `index.html` | The entire app |
| `manifest.json` | PWA metadata (name, colors, icons) |
| `sw.js` | Service worker — enables offline use |
| `icon-192.png` | App icon (home screen) |
| `icon-512.png` | App icon (splash screen) |

## Data
Scenarios are saved to your browser's local storage — they persist between sessions and survive app restarts, but are stored on-device only.
