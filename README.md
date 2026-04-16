# drop — Free fall simulation

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

Remote repo: [github.com/dr-sad/drop](https://github.com/dr-sad/drop)

If this folder is **not** yet linked to GitHub:

```powershell
cd "C:\Users\Stephanie.Sadrian\Documents\Vibe Coding\MikeSIM"
git init
git branch -M main
git add MikeSIM_SNS.html index.html README.md
git commit -m "Add free fall simulation and local preview files"
git remote add origin https://github.com/dr-sad/drop.git
```

If the GitHub repo **already has commits** (for example an older `MikeSIM_SNS.html`), pull and merge once, then push:

```powershell
git pull origin main --allow-unrelated-histories
git push -u origin main
```

If GitHub asks you to sign in, use **GitHub Desktop**, **SSH**, or a **personal access token** when prompted for a password over HTTPS.

## Optional: host a live preview (GitHub Pages)

1. Push the files above to the `main` branch on `dr-sad/drop`.
2. On GitHub: **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, branch **main**, folder **/ (root)**.
4. After a minute, the site will be at:

   **https://dr-sad.github.io/drop/**

`index.html` redirects visitors to `MikeSIM_SNS.html`.
