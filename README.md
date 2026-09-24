# URIS STEM Vocabulary Website — Version 0.5

A lightweight static website for the PolyU URIS STEM Vocabulary research project.

## Open locally

Open `index.html` directly in a browser. Search, filters, sorting, and the Affix Explorer require no installation. For a local-server preview, run `python3 -m http.server 8000` inside this folder and open `http://localhost:8000/`.

## Pages

- `index.html` — project introduction and APA website citation
- `vocabulary.html` — four searchable vocabulary sets
- `affixes.html` — affix explorer centred on the 34-word study set
- `outputs.html` — embedded conference presentation, citation, and space for future publications
- `news.html` — project news and announcements
- `team.html` — three-member team page and profile links
- `about.html` — research rationale, source lineage, and selected references

Shared files are `css/style.css`, `js/main.js`, and `data/vocabulary.js`. Full data provenance is recorded in `data/SOURCES.md`.

## Data integrity

The website contains no participant-level data. Original URIS research files remain read-only. The 34-word current study set includes its verified morphological categories and split prefix/suffix fields. The 138-word candidate pool displays only the affix coding already recorded in the candidate-pool source, separated into prefix and suffix columns; missing values are shown as `NA`.

## Dependencies

None. The site uses HTML, CSS, vanilla JavaScript, a system Avenir/Helvetica/Arial font stack, and one compact local data file. There is no framework, package manager, build step, analytics, database, or external runtime dependency.

The PolyU logo in `assets/images/polyu-logo.png` is the unmodified public 1× asset served by the official PolyU website. The conference presentation is displayed through the browser's built-in PDF viewer using the unchanged file in `assets/outputs/polyu-calls-2025.pdf`.

## Deployment

GitHub Pages can publish the repository directly from the `main` branch without a build command. Future changes are made by updating the same files and committing them to the repository; GitHub Pages then republishes automatically. A custom domain can be connected later through the repository’s Pages settings.

## Deferred work for the next data update

- Receive the researcher-reviewed Excel classification for the broader 138-word pool before adding morphological categories or further affix coding beyond the recorded source fields.
- Confirm the remaining 28 context-sensitive POS entries before replacing their `Pending verification` labels. The local review workbook is excluded from GitHub publishing.
- Review the optimized team portraits if updated source photos are supplied later.
