# UNAB Winter School website

Starter repository for a GitHub Pages website.

## Publish with GitHub Pages

1. Create a new public GitHub repository, for example `winter-school-2027`.
2. Upload all files in this folder to the repository root.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`.
6. Save. GitHub will publish the site at:
   `https://YOUR-USERNAME.github.io/winter-school-2027/`
7. Set `baseurl: "/winter-school-2027"` in `_config.yml` unless the repository is your main `USERNAME.github.io` site.

## Recommended workflow

- Put PDFs in `materials/`.
- Put data files in `datasets/`.
- Put exercises in `exercises/`.
- Create one Markdown page per course in `courses/`.
- Replace all `[PLACEHOLDER]` text before publication.

## Local preview

GitHub Pages uses Jekyll. A local preview is optional; the easiest workflow is to edit Markdown directly in GitHub and use the deployed site as preview.
