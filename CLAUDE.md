# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

See `AGENTS.md` for the full contributor guide (project structure, coding style, commit conventions). This file adds the architecture context and gotchas specific to working here.

## What this is

A personal academic site built on Hugo + the HugoBlox "Academic CV" theme, deployed to GitHub Pages at `https://praeclarumjj3.github.io`. Requires **Hugo Extended**; CI pins `0.126.3` (`hugoblox.yaml`, `.github/workflows/publish.yaml`).

## Commands

- `hugo server -D` — local dev with drafts enabled.
- `hugo --minify` — production build into `public/`.
- `hugo --minify --baseURL "https://praeclarumjj3.github.io/"` — verify production URLs before deploying.
- `npx pagefind --site public` — regenerate the search index after a production build (matches the Pages workflow).

There is no unit test suite. `hugo --minify` (plus a local `hugo server -D` visual check for layout/nav changes) is the validation step.

## Architecture — the non-obvious parts

- **The theme is a Go module, not vendored.** `config/_default/module.yaml` imports `blox-tailwind` and `blox-plugin-netlify`; `blox-bootstrap` comes in transitively (see `go.mod`). Layouts, partials, and styles you never see in this repo live inside those modules' Hugo module cache. `layouts/` here holds *only overrides* (currently a single head-end hook), and `module.yaml` `mounts` map local `layouts/`/`assets/` over the module's.

- **`public/` is committed generated output.** Unlike most Hugo repos, the built site is tracked in git — that's why editing any content produces a large `public/` diff. Never hand-edit files under `public/`; regenerate them by running Hugo and commit the result alongside the source change.

- **Two deploy workflows exist.** `.github/workflows/gh-pages.yaml` (Hugo `latest`, `hugo --minify`, pushes `public/` via `actions-gh-pages`) and `.github/workflows/publish.yaml` (pinned `0.126.3`, builds with the Pages base URL, then runs Pagefind). Keep changes to either minimal.

- **Publications can be auto-imported.** Pushing/updating a `publications.bib` file triggers `.github/workflows/import-publications.yml`, which runs the `academic` CLI to generate `content/publication/*` markdown and opens a PR. Prefer editing the `.bib` over hand-writing publication pages when that flow applies.

## Content layout

Editable source is under `content/`: `blogs/`, `project/`, `publication/`, `experience.md`, and author/profile data in `content/authors/admin/`. Each publication/project entry is a folder with `index.md` plus co-located assets (`featured.png`, `cite.bib`). Site config is in `config/_default/` (`hugo.yaml`, `menus.yaml`, `params.yaml`, `module.yaml`, `languages.yaml`).

`static/` holds **standalone project demo sites** (e.g. `oneformer/`, `sage/`, `vcoder/`, `fcf-inpainting/`) — self-contained HTML/asset bundles that Hugo copies verbatim into the output; they are not driven by the Hugo templates.

## Conventions

Use short, lowercase, hyphenated slugs for new folders/files (`content/publication/new-paper/index.md`). Two-space YAML indentation; match front matter to neighboring files. Avoid unrelated formatting churn in `public/`.
