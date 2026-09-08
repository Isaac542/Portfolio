# Portfolio site template

A simple 3-project portfolio site, styled like an engineering drawing sheet
(title block header, sheet numbers, hairline rules). Pure HTML/CSS — no
build step, no dependencies beyond Google Fonts.

## File structure

```
index.html                     ← homepage / project index
projects/
  project-1.html                ← project page 1
  project-2.html                ← project page 2
  project-3.html                ← project page 3
assets/
  style.css                     ← all styling, shared by every page
  images/project-1/             ← drop project 1's images here
  images/project-2/
  images/project-3/
  files/project-1/               ← drop project 1's downloadable files here
  files/project-2/
  files/project-3/
```

## Customizing

1. **Your name and links** — in `index.html` and each `projects/project-N.html`,
   replace `JORDAN REYES`, the email address, and the LinkedIn/GitHub links in
   the header and hero.
2. **Homepage copy** — edit the hero paragraph and the three rows under
   "SHEET INDEX" in `index.html` (title, one-line description, tags).
3. **Each project page** has three editable sections, marked with HTML
   comments in the file:
   - **Text** — the `OVERVIEW` section: a couple of paragraphs plus a bullet
     list of key points.
   - **Images** — the `FIGURES` gallery. Drop image files into the matching
     `assets/images/project-N/` folder, then swap the placeholder
     `<div class="plate-empty">...</div>` line for an `<img>` tag (the
     exact syntax to use is left in a comment right above each figure).
   - **Files** — the `ATTACHMENTS` table. Drop PDFs, CAD exports, or
     spreadsheets into `assets/files/project-N/`, then update the file names
     and links in the table rows (add or delete `<tr>` rows as needed).
4. **Optional video** — each project page has a commented-out YouTube embed
   block under `WALKTHROUGH`. Uncomment it and swap in your video ID (the
   part of a YouTube URL after `watch?v=`) if you want to embed a walkthrough
   or simulation clip.
5. **Renaming projects** — the nav bar and pager links on every page
   currently read "PROJECT NAME". Do a find-and-replace for that placeholder
   text across all four HTML files once you've settled on real project
   titles, so the navigation matches the homepage.

## Publishing with GitHub Pages

1. Create a new repository on GitHub (public, or private if you have GitHub
   Pro/Team — public repos get free Pages on any plan).
2. Upload all the files in this folder to the repository, keeping the same
   folder structure.
3. In the repository, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch",
   choose the `main` branch and the `/ (root)` folder, then save.
5. GitHub will give you a URL like `https://yourusername.github.io/repo-name/`
   within a minute or two. That's your live site.
6. Optional: to use a custom domain, add it under **Settings → Pages →
   Custom domain** and follow GitHub's DNS instructions.

Any time you push changes to the branch you deployed from, the live site
updates automatically within a minute or so.
