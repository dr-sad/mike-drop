# mike-drop — Free fall simulation

Static HTML simulation for learning about gravity and air resistance.

## Preview on your computer

From this folder, start a small local web server (browsers work best with **http://** URLs, not `file://`).

**Python 3** (already installed on many PCs):

```powershell
cd "C:\Users\Stephanie.Sadrian\Documents\Vibe Coding\MikeSIM"
python -m http.server 8080
```

Then open **http://localhost:8080/** or **http://localhost:8080/MikeSIM_SNS.html** in your browser.

**Node.js** (alternative):

```powershell
npx --yes serve -l 8080
```

Follow the URL printed in the terminal (often **http://localhost:8080**).

## Put your changes on GitHub

Remote repo: [github.com/dr-sad/mike-drop](https://github.com/dr-sad/mike-drop)

If this folder is **not** yet linked to GitHub:

```powershell
cd "C:\Users\Stephanie.Sadrian\Documents\Vibe Coding\MikeSIM"
git init
git branch -M main
git add MikeSIM_SNS.html index.html README.md
git commit -m "Add free fall simulation and local preview files"
git remote add origin https://github.com/dr-sad/mike-drop.git
```

If the GitHub repo **already has commits** (for example an older `MikeSIM_SNS.html`), pull and merge once, then push:

```powershell
git pull origin main --allow-unrelated-histories
git push -u origin main
```

If GitHub asks you to sign in, use **GitHub Desktop**, **SSH**, or a **personal access token** when prompted for a password over HTTPS.

## Optional: host a live preview (GitHub Pages)

1. Push the files above to the `main` branch on `dr-sad/mike-drop`.
2. On GitHub: **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, branch **main**, folder **/ (root)**.
4. After a rename, open **Pages** once and confirm the source is still **main / (root)**; GitHub may need a minute to republish.
5. The site URL uses the **repository name**. After renaming `drop` → `mike-drop`, use:

   **https://dr-sad.github.io/mike-drop/**

   Old links like `https://dr-sad.github.io/drop/` will no longer load the site.

`index.html` redirects visitors to `MikeSIM_SNS.html`.

## Embed snippet (direct file URL)

Use this snippet to embed the simulation directly (recommended):

```html
<iframe
  src="https://dr-sad.github.io/mike-drop/MikeSIM_SNS.html"
  width="850"
  height="540"
  style="border:0; max-width:100%;"
  loading="lazy"
  allowfullscreen
  title="Mike Drop Simulation">
</iframe>
```

Direct-linking to `MikeSIM_SNS.html` avoids redirect hiccups that can happen when embedding the repo root URL.
