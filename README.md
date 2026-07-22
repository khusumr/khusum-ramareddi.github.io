# Khusum Ramareddi — Resume Site

A single-page resume site styled like API documentation (fitting, since it's built with
FastAPI/Azure experience). Plain HTML, CSS, and JavaScript — no frameworks, no build step.

## Files
- `index.html` — page content
- `style.css` — all styling
- `script.js` — scroll-reveal animation

---

## Step 1 — Open the project in VS Code

1. Unzip / save this folder somewhere you'll remember (e.g. Desktop/resume-site).
2. Open **VS Code**.
3. `File > Open Folder...` → select the `resume-site` folder.
4. You should see `index.html`, `style.css`, and `script.js` in the sidebar.

## Step 2 — Preview it locally

Easiest way: in VS Code's file explorer, right-click `index.html` → **"Reveal in File Explorer / Finder"**,
then just double-click the file to open it in your browser.

Nicer way (auto-refreshes when you edit):
1. In VS Code, go to the Extensions icon (left sidebar, looks like 4 squares).
2. Search **"Live Server"** by Ritwick Dey → click **Install**.
3. Right-click `index.html` in the file list → **"Open with Live Server"**.
4. It opens in your browser at something like `http://127.0.0.1:5500` and refreshes automatically when you save changes.

## Step 3 — Create a GitHub repository

1. Go to [github.com](https://github.com) and log in.
2. Click the **+** icon (top right) → **New repository**.
3. Name it exactly: `khusum-ramareddi.github.io`
   *(Naming it `yourusername.github.io` makes GitHub Pages publish it automatically at the root URL,
   instead of a `/repo-name/` subpath — cleaner for a resume link.)*
4. Keep it **Public**.
5. Do **NOT** check "Add a README" (we already have one).
6. Click **Create repository**. Keep this page open — the next screen shows you commands.

## Step 4 — Push your code to GitHub

Open a terminal **inside VS Code**: `Terminal > New Terminal` (top menu). Make sure you're inside
the `resume-site` folder (it should say so in the terminal prompt), then run these commands
one at a time:

```bash
git init
git add .
git commit -m "Initial resume site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/khusum-ramareddi.github.io.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your actual GitHub username. If this is your **first time** using
git from this computer, it may ask you to log in — a browser window will pop up to authenticate;
just follow the prompts.

If `git` isn't recognized at all, you need to install it first: [git-scm.com/downloads](https://git-scm.com/downloads),
then restart VS Code and try again.

## Step 5 — Turn on GitHub Pages

1. On your repository's GitHub page, click **Settings** (top tab).
2. In the left sidebar, click **Pages**.
3. Under **Build and deployment > Source**, choose **Deploy from a branch**.
4. Under **Branch**, choose `main` and folder `/ (root)` → click **Save**.
5. Wait about 1 minute, then refresh the page. GitHub will show a green box with your live URL —
   something like:

   `https://YOUR-USERNAME.github.io/`

   (or `https://YOUR-USERNAME.github.io/khusum-ramareddi.github.io/` if you named the repo
   something other than `username.github.io` — the repo name above avoids that.)

That link is now your live resume site. Put it on your actual resume, LinkedIn, and job applications.

## Making future changes

Whenever you edit the files and want to update the live site:

```bash
git add .
git commit -m "describe what you changed"
git push
```

GitHub Pages will redeploy automatically within a minute or two.
