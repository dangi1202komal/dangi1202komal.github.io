# Komal Dangi portfolio

Website: https://jatindangi1206.github.io/komal/

## Files

- `index.html` is the complete website, including bundled scripts, fonts, and image.
- `.github/workflows/deploy-pages.yml` publishes it to GitHub Pages.

No package installation or build command is needed. The bundled page requires JavaScript in a modern browser.

## Preview locally

From this folder, run:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000 and press Ctrl+C to stop the server.

## Publish updates

Edit or replace `index.html`, then commit and push to `main`:

```sh
git add index.html
git commit -m "Update portfolio"
git push
```

GitHub Actions deploys every push to `main`. You can also run the workflow manually from the repository's Actions tab. In Settings → Pages, the source must be **GitHub Actions**.

The workflow uploads only `index.html`. If you add separate assets later, include them in the workflow's Prepare website step too.
