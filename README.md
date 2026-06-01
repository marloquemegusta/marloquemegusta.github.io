# Mario Alfonso Arsuaga personal website

Static personal academic/technical website built with plain HTML, CSS, Bootstrap, and a small amount of JavaScript.
There is no build step: GitHub Pages can serve the repository root directly.

## Local preview

Open `index.html` directly in a browser, or serve the folder with any static server:

```powershell
python -m http.server 8000
```

Then visit `http://localhost:8000/`.

## Structure

- `index.html`: main personal website.
- `index_dynerfactor.html`, `index_neuralux.html`, `index_physplat.html`: project pages.
- `css/`, `javascript/`: site styles and scripts.
- `imgs/`, `gifs/`, `videos/`: media assets.

All internal assets and project pages use relative paths, so the site can be deployed either at a GitHub Pages root
domain or as a project page.

## Recommended migration

Preferred destination:

- Repository: `marloquemegusta.github.io`
- URL: `https://marloquemegusta.github.io/`

This is the cleanest option because the current site does not require a project-page base path such as
`/marioalfonsoarsuaga/`.

Suggested migration commands:

```powershell
git remote rename origin old-origin
git remote add origin https://github.com/marloquemegusta/marloquemegusta.github.io.git
git push -u origin main
```

Then configure GitHub Pages in the new repository:

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/ (root)`

Keep the old `malfonsoarquimea/marioalfonsoarsuaga` deployment unchanged until the new URL has been tested.
After validation, the old repository can serve a simple redirect page to `https://marloquemegusta.github.io/`.

## Migration notes

- Canonical URL in `index.html` points to `https://marloquemegusta.github.io/`.
- Public links were updated to emphasize the personal GitHub identity `marloquemegusta`.
- No framework migration was performed; the site remains a lightweight static website.
