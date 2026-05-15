# Repository Guidelines

## Project Structure & Module Organization

This repository is a Hugo/HugoBlox academic site. Primary editable content lives in `content/`: blog posts in `content/blogs/`, projects in `content/project/`, publications in `content/publication/`, and profile data in `content/authors/admin/`. Site settings are under `config/_default/`, with navigation in `menus.yaml`, theme/module imports in `module.yaml`, and general Hugo settings in `hugo.yaml`. Static project pages and standalone assets live in `static/`; Hugo copies them into the generated site. `assets/` contains Hugo pipeline assets, while `layouts/` is for template overrides. `public/` is generated output for the deployed site; update it only by running Hugo, not by hand-editing HTML.

## Build, Test, and Development Commands

- `hugo server -D`: run the site locally with draft content enabled.
- `hugo --minify`: build the production site into `public/`.
- `hugo --minify --baseURL "https://praeclarumjj3.github.io/"`: verify production URLs before deployment.
- `npx pagefind --site public`: regenerate the search index after a production build, matching the GitHub Pages workflow.

Use Hugo Extended. The published workflow pins Hugo `0.126.3` in `.github/workflows/publish.yaml`.

## Coding Style & Naming Conventions

Write Markdown content with YAML/TOML front matter consistent with neighboring files. Prefer short, lowercase slugs for new folders and filenames, using hyphens where needed, for example `content/publication/new-paper/index.md`. Keep YAML indentation at two spaces. Store publication assets beside their `index.md` as `featured.png` and `cite.bib` when applicable. Avoid large unrelated formatting changes in generated `public/` files.

## Testing Guidelines

There is no dedicated unit test suite. Treat `hugo --minify` as the required validation step for content and config changes. For visual or navigation changes, also run `hugo server -D` and inspect the affected page locally. Check the generated output for broken links, missing images, malformed front matter, and unexpected changes in `public/`.

## Commit & Pull Request Guidelines

Recent history uses short imperative or summary commits such as `update`, `Build SAGE Project for Release`, and `Finalize SAGE releasse`. Prefer clearer messages in the same concise style, for example `Update SAGE publication page` or `Add project thumbnail`. Pull requests should describe the content or config changed, list validation commands run, link related issues when available, and include screenshots for visible page updates.

## Security & Configuration Tips

Do not commit secrets, tokens, unpublished private PDFs, or local machine paths. Keep deployment changes in `.github/workflows/` minimal and verify GitHub Pages settings before changing `baseURL` or workflow permissions.
