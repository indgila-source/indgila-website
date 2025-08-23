# Full‑Bleed Portfolio (Starter)
A super-minimal, single-file website with:
- full-screen images (cover fit)
- left/right zone navigation with [prev]/[next]
- randomized order on each load
- caption at bottom-right
- “INFORMATION” overlay (bio + publications)

## How to use
1) Put your large images into the `images/` folder (JPG/PNG, ~2400px wide).
2) Open `index.html` and edit the `slides` array near the bottom:
   ```js
   const slides = [
     { src: 'images/01.jpg', caption: 'Title — short description.' },
     { src: 'images/02.jpg', caption: '...' },
   ];
   ```
3) Edit the “INFORMATION” overlay content inside `index.html` (bio, publications, links).
4) Double-click `index.html` to preview locally.

## Deploy (fastest options)
- **Netlify Drop:** go to https://app.netlify.com/drop and drag the entire folder in.
- **GitHub Pages:** create a repo, upload files, enable Pages in repo settings.
- **Vercel:** create account → “New Project” → import from GitHub (or drag-and-drop).

## Update later
Just replace/add images in `images/` and update the `slides` array. Order randomizes automatically on each visit.

## Notes
- Keyboard arrows work (← →). On touch, tap left/right side to navigate.
- If you don’t want random order, delete the `shuffle(slides);` line in the script.
- Big images = nicer quality; try to keep files 400–800 KB each for fast loads.
