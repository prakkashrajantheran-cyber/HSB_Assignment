# Thalassemia Guide for Future Parents

A simple, family-friendly website about thalassemia carrier status, blood-report terms, and family planning.

Includes:
- 60-second animated video (oxygen-truck analogy)
- 5 parent podcast episodes (ready to play – no zip needed)

**Total size ~7–8 MB** so it uploads easily to GitHub.

---

## Folder structure

```
thalassemia-github/
├── index.html
├── README.md
├── .gitignore
├── .nojekyll
└── media/
    ├── thalassemia_parent_guide_60s.mp4
    ├── Episode_1_with_music.mp3
    ├── Episode_2_with_music.mp3
    ├── Episode_3_with_music.mp3
    ├── Episode_4_with_music.mp3
    └── Episode_5_with_music.mp3
```

---

## Open in VS Code

1. Unzip this folder.
2. Open the folder in VS Code.
3. Install the **Live Server** extension (Ritwick Dey).
4. Right-click `index.html` → **Open with Live Server**.

Go to **Videos and podcast** — the video and all 5 episodes play immediately.

---

## Upload to GitHub (easy way)

### Option A – GitHub website (drag & drop)

1. Go to [github.com](https://github.com) and create a **new repository**.  
   Example name: `thalassemia-parent-guide`  
   Leave it **empty** (no README, no .gitignore).

2. On the empty repository page click **uploading an existing file**.

3. Drag **all the files and the `media` folder** into the browser window  
   (or select everything inside the `thalassemia-github` folder).

4. Click **Commit changes**.

5. Go to **Settings → Pages**.

6. Under **Source** choose:
   - Branch: `main`
   - Folder: `/ (root)`

7. Click **Save**.

8. Wait 1–2 minutes. Your site will be live at:

   ```
   https://YOUR-USERNAME.github.io/thalassemia-parent-guide/
   ```

### Option B – Using Git in VS Code / Terminal

```bash
cd thalassemia-github
git init
git add .
git commit -m "Thalassemia Parent Guide – ready for GitHub Pages"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/thalassemia-parent-guide.git
git push -u origin main
```

Then enable GitHub Pages (Settings → Pages) as above.

---

## Notes

- All media files are already inside the `media` folder.
- Paths are relative (`media/...`) so they work both locally and on GitHub Pages.
- No backend, no build step — pure HTML/CSS/JS.
- Theme (Light / Dark / System) is saved in the browser.
- This is general educational information only, not medical advice.
