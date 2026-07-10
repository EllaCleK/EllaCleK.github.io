# Portfolio v2 — HTML5 + CSS, multi-page

This version splits your site into proper files (like Nate's repo):

    index.html                     ← main page (HTML5)
    style.css                      ← ALL styling (CSS3), shared by every page
    .nojekyll                      ← tells GitHub Pages to serve files as-is
    projects/
      built-on-truss.html          ← full project page
      solar-car.html               ← full project page
      built-on-truss/  (images)

The homepage now shows PREVIEW CARDS in the Projects section; clicking a card
opens that project's own full page. Exactly the "both" setup you asked for.

------------------------------------------------------------------------
## How to update your repo (github.com/ellaclek/ellaclek.github.io)
------------------------------------------------------------------------

Your repo currently has the single-file version. We're replacing it with these
files. Cleanest path:

1. Delete the current top-level files in the repo (index.html, SETUP-GUIDE.md).
   Leave the projects/ folder and .nojekyll — we'll overwrite/add.
   - For each file: click it → trash-can icon (or ... → Delete file) → Commit.

2. Upload the new files. On the repo main page:
   - "Add file" → "Upload files"
   - From this unzipped folder, drag in EVERYTHING:
     index.html, style.css, .nojekyll, and the projects folder.
   - GitHub will show them merging into place. Check that you see:
       index.html
       style.css
       projects/built-on-truss.html
       projects/solar-car.html
       projects/built-on-truss/ (the images)
   - Commit changes.

3. That's it — Pages is already on from before. Wait ~1-2 min, hard-refresh
   (Ctrl+F5) https://ellaclek.github.io

If GitHub won't let you overwrite index.html during upload, delete the old
index.html first (step 1), then upload.

------------------------------------------------------------------------
## Résumé button
------------------------------------------------------------------------
Both the home hero and the button point to  assets/resume.pdf
Upload your PDF there:
  - "Add file" → "Create new file" → type  assets/README.txt  → "x" → commit
    (this makes the assets folder), THEN open assets/, "Add file" → "Upload
    files", drag resume.pdf in, commit.
  - Or give me a Google Drive link and I'll change the button to point at it.

------------------------------------------------------------------------
## Adding a new project later (easy pattern)
------------------------------------------------------------------------
1. Copy projects/solar-car.html to projects/your-project.html and edit the text.
2. Add its images to projects/your-project/  and update the <img src> paths.
3. On index.html, copy one <a class="proj-card"> block in the Projects section,
   point its href to projects/your-project.html, set the thumbnail + title.
Send me the details and photos and I'll generate the page for you.
