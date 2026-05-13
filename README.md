# Salmon River Tubing — GitHub Pages Site

Website for **salmonrivertubing.com** — tube and kayak rentals at Steelhead Lodge, Pulaski, NY.

---

## File Structure

```
/
├── index.html          ← Main homepage (all 6 sections)
├── css/
│   └── styles.css      ← All styles (river blues, greens, wood tones)
├── images/             ← Add your photos here (see below)
│   ├── hero.jpg        ← Hero background (1920×1080 minimum, people tubing)
│   ├── tubing-action.jpg ← "Why Float" section photo
│   └── og-hero.jpg     ← Open Graph / social share image (1200×630)
└── README.md
```

---

## Deploy to GitHub Pages (Step by Step)

### 1. Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in (or create a free account).
2. Click **+** → **New repository**.
3. Name it: `salmonrivertubing` (or anything you like).
4. Set it to **Public**.
5. Click **Create repository**.

### 2. Upload Your Files

**Option A — Drag & Drop (easiest):**
1. On your new repo page, click **uploading an existing file**.
2. Drag in `index.html`, the `css/` folder, and the `images/` folder.
3. Click **Commit changes**.

**Option B — Git command line:**
```bash
git init
git add .
git commit -m "Initial site — Salmon River Tubing"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/salmonrivertubing.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. In your repo, go to **Settings** → **Pages** (left sidebar).
2. Under **Source**, select **Deploy from a branch**.
3. Choose branch: **main**, folder: **/ (root)**.
4. Click **Save**.
5. Your site will be live in ~60 seconds at:
   `https://YOUR-USERNAME.github.io/salmonrivertubing/`

### 4. Connect Your GoDaddy Domain

1. In GitHub Pages settings, enter `salmonrivertubing.com` under **Custom domain** and click Save.
2. GitHub will create a `CNAME` file automatically.
3. In **GoDaddy DNS** (Domain → DNS), add these records:

| Type  | Name | Value                  |
|-------|------|------------------------|
| A     | @    | 185.199.108.153        |
| A     | @    | 185.199.109.153        |
| A     | @    | 185.199.110.153        |
| A     | @    | 185.199.111.153        |
| CNAME | www  | YOUR-USERNAME.github.io |

4. Check **Enforce HTTPS** in GitHub Pages settings (may take up to 24 hours for DNS to propagate).

---

## Add Your Photos

Replace placeholders with real photos for best results:

- **`images/hero.jpg`** — Big action shot of people tubing/kayaking on the Salmon River. Landscape, 1920×1080 or larger.
- **`images/tubing-action.jpg`** — A candid river photo for the "Why Float" section. Approx 800×600.
- **`images/og-hero.jpg`** — Cropped to 1200×630 for Facebook/Twitter previews.

Once added, the placeholders will automatically be replaced by your images.

---

## Customizations

| What to change | Where |
|---|---|
| Phone number | Search & replace `3152984371` in `index.html` |
| Google Maps embed | Replace the `<iframe src="...">` in the contact section |
| Package prices | Edit the `.card-price` values in index.html |
| Release dates | Update the `<ul class="release-dates">` list |
| Book Now link | Replace `href="tel:3152984371"` with LodgeRunner or booking URL |

---

## Questions?

Call Steelhead Lodge: **(315) 298-4371**
