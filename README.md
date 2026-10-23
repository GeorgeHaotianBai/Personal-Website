# George Bai academic website

The website at https://georgebai.com currently shows a single under-construction page. The page lives in `site/`, and `.github/workflows/deploy.yml` publishes that folder through GitHub Pages whenever `main` changes. The same page also serves as the 404 page.

## Archived site

The full Hugo site, as it was live on 23 October 2026, is kept in the tag `archive-2026-10-23` and in the branch `archived-site-2026-10-23`. Both point to commit `9a16cb0`.

## Restoring the archived site

From a clone of this repository, run:

```bash
git checkout main
git checkout archive-2026-10-23 -- .
git rm -r -q site
git commit -m "Restore archived site"
git push
```

The restored workflow then rebuilds the Hugo site and publishes it to https://georgebai.com.
