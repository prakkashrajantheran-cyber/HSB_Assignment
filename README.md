# Thalassemia Guide for Future Parents

A clear, family-friendly website that explains thalassemia carrier status, blood-report terms (MCV, MCH, etc.), inheritance chances, and includes:

- A 60-second animated video (oxygen-truck analogy)
- 5 parent podcast episodes (ready to play – no zip download needed)

## Folder structure

```
thalassemia-site/
├── index.html          ← the whole website
├── README.md
├── .gitignore
├── .nojekyll           ← needed for GitHub Pages
└── media/
    ├── thalassemia_parent_guide_60s.mp4   ← video
    ├── Episode_1_with_music.mp3
    ├── Episode_2_with_music.mp3
    ├── Episode_3_with_music.mp3
    ├── Episode_4_with_music.mp3
    └── Episode_5_with_music.mp3
```

## Open in VS Code (local testing)

1. Open the folder `thalassemia-site` in VS Code.
2. Install the **Live Server** extension (by Ritwick Dey) if you don’t have it.
3. Right-click `index.html` → **Open with Live Server**.

The site opens in your browser.  
Go to **Videos and podcast** → the video and all 5 podcast episodes play immediately.

## Host free on GitHub Pages

### Step-by-step

1. Create a new repository on GitHub  
   Example name: `thalassemia-parent-guide`

2. Upload **everything** inside the `thalassemia-site` folder  
   (you can drag-and-drop the whole folder contents into the GitHub web uploader, or use Git).

3. Go to the repository **Settings** → **Pages**.

4. Under **Source** choose:
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`

5. Click **Save**.

6. Wait 1–2 minutes. GitHub will give you a link like:

   ```
   https://your-username.github.io/thalassemia-parent-guide/
   ```

The video and all podcast episodes will work because the paths are relative (`media/...`) and the files are already in the repository.

### Using Git (optional, for VS Code)

```bash
cd thalassemia-site
git init
git add .
git commit -m "Initial commit – Thalassemia Parent Guide"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/thalassemia-parent-guide.git
git push -u origin main
```

Then enable GitHub Pages as described above.

## Notes

- All media files are already included in the `media` folder.
- No zip file is needed – the podcasts play directly.
- Theme (Light / Dark / System) is remembered in the browser.
- Pure HTML / CSS / JS – no build step, no backend.
- Works offline once the page has loaded (except Google Fonts).
