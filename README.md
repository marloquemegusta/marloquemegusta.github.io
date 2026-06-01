# Mario Alfonso Arsuaga personal website

This repository contains the current version of my personal academic and technical website:

https://marloquemegusta.github.io/

It is the continued personal version of my previous website, now maintained under my personal GitHub account.

The site is intentionally simple: plain HTML, CSS, Bootstrap, and a small amount of JavaScript. There is no build step.

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

## Deployment

The site is served with GitHub Pages from the `main` branch and repository root.
