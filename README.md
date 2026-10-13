# Personal website: Cicy K. Agnes

A plain HTML/CSS academic homepage for GitHub Pages. There's no build step, and Jekyll and Ruby aren't needed.

```
index.html            Home: bio, research interests, news, collaborate
publications.html     All publications, grouped by year, with BibTeX
404.html              Page-not-found page
assets/css/style.css  All styling (light and dark mode, mobile layout)
images/profile.svg    Placeholder avatar (initials)
images/profile.jpg    <- add your photo here (square works best)
files/CV.pdf          <- add your CV here
.nojekyll             Tells GitHub Pages to serve the files as they are
```

## Publish in 5 minutes

1. Create a **public** repository on GitHub named exactly `YOUR-GITHUB-USERNAME.github.io`.
2. Upload every file in this folder, including the hidden `.nojekyll` file. Use **Add file → Upload files**, or:
   ```bash
   git init
   git add .
   git commit -m "Personal website"
   git branch -M main
   git remote add origin https://github.com/YOUR-GITHUB-USERNAME/YOUR-GITHUB-USERNAME.github.io.git
   git push -u origin main
   ```
3. In the repository, go to **Settings → Pages**. Set **Source** to *Deploy from a branch*, then choose **Branch** `main` and folder `/ (root)`.
4. After a minute or two, the site is live at `https://YOUR-GITHUB-USERNAME.github.io`.

To preview it locally, just open `index.html` in a browser.

## Before you publish: fill in these placeholders

Search all files for these strings and replace them. Each one appears in both `index.html` and `publications.html`.

| Placeholder | Replace with |
| --- | --- |
| `YOUR-GITHUB-USERNAME` | Your GitHub username |
| `YOUR-SCHOLAR-ID` | The `user=` value from your Google Scholar profile URL |

Also:

- **Photo:** save a square photo as `images/profile.jpg`. Until you do, the initials placeholder is shown.
- **CV:** save your CV as `files/CV.pdf`. You may want to remove your phone number from the public version.
- **Email:** the site uses `cicyagnes@gmail.com`, taken from your CV. Check that it's the address you want shown.
- **Paper links:** each publication has a comment showing where to add `arXiv`, `PDF` or `Code` buttons.

## Editing

- **Add a news item:** in `index.html`, copy a line like
  `<li><span class="date">[Oct'26]</span> Text here.</li>` and put it at the top of the News list. Move older items into
  the collapsible **Old** list below it.
- **Add a publication:** in `publications.html`, copy a whole `<div class="pub">…</div>` block and edit the title,
  authors (wrap your name in `<span class="me">`), venue badge, optional one-line summary and BibTeX.
- **Colours and fonts:** all colours live at the top of `assets/css/style.css` as variables, with a matching dark-mode set.

Icons are from Font Awesome Free 6.5.2 (CC BY 4.0) and are embedded in the pages, so the site loads nothing from
external servers.
