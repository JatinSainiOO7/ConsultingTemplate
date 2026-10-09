# ResearchVista website (build)

Compiled, prerendered build of the ResearchVista consultancy website (Angular 22), prepared for GitHub Pages at:

https://jatinsainioo7.github.io/ConsultingTemplate/

This repository holds the build output only. The source code is kept in the separate Angular project.

## Publish

In this repository on GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main`, folder: `/ (root)` → Save.** The site is live a minute or two later.

## Update the site

1. In the source project, build with this repository's path as the base:
   `npx ng build --base-href /ConsultingTemplate/`
   (run it in PowerShell or cmd; Git Bash rewrites the path).
2. From `dist/researchvista/browser`, copy `index.csr.html` to `404.html`.
3. Replace the files in this repository with the new build, keeping `.nojekyll` and this README, then commit and push.

`404.html` lets the admin page and mistyped addresses load the site instead of GitHub's error page. `.nojekyll` stops GitHub from processing the files.
