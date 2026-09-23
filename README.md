# URIS STEM Vocabulary Website — Version 0.4

A lightweight static website for the PolyU URIS STEM Vocabulary research project.

## Open locally

Open `index.html` directly in a browser. Search, filters, sorting, and the Affix Explorer require no installation. For a local-server preview, run `python3 -m http.server 8000` inside this folder and open `http://localhost:8000/`.

## Pages

- `index.html` — concise project introduction
- `vocabulary.html` — four searchable vocabulary sets
- `affixes.html` — 34-word core affix explorer with selected background examples
- `team.html` — three-member team page and profile links
- `about.html` — research rationale, source lineage, and status

Shared files are `css/style.css`, `js/main.js`, and `data/vocabulary.js`. Full data provenance is recorded in `data/SOURCES.md`.

## Data integrity

The website contains no participant-level data. Missing POS or Traditional Chinese terminology is explicitly marked for verification and is never guessed. Original URIS files remain read-only.

## Dependencies

None. The site uses HTML, CSS, vanilla JavaScript, a system Avenir/Helvetica/Arial font stack, and one compact local data file. There is no framework, package manager, build step, analytics, database, or external runtime dependency.

The compact PolyU logo in `assets/images/polyu-logo.png` is the unmodified public 1× asset served by the official PolyU website (`https://www.polyu.edu.hk/assets/img/main-logo-1x.png`). It links to the University homepage.

## Deployment

Upload this folder to a static host. GitHub Pages is the simplest free option; Cloudflare Pages and Netlify also work without a build command. A short custom URL can later be connected through the selected host. No deployment or domain configuration has been performed.

## Recommended Version 0.5 direction

Review the remaining `待核實` terminology, replace the three photo placeholders with approved optimized portraits, and confirm whether the public resource should retain all source-list words or foreground a smaller pedagogical subset.
