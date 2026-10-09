# Mohammad Alvi Refat — Industry Résumé

Editable LaTeX source for a one-page scientific-computing résumé.

## Compile

Compile locally with PDFLaTeX:

```sh
latexmk -pdf Mohammad_Alvi_Refat_Resume.tex
```

On Overleaf, set `Mohammad_Alvi_Refat_Resume.tex` as the main document and
select PDFLaTeX.

## Automatic website update

This project is kept in the separate `MohammadRefat23/resume` GitHub
repository. Its `.github/workflows/trigger-website.yml` workflow dispatches the
website repository's `deploy.yml` after a push to `main`. The website workflow
checks out this repository alongside `MohammadRefat23/cv`, compiles both PDFs,
and deploys them with the site. Add a `WEBSITE_ACTION_TOKEN` secret in this
repository with permission to dispatch workflows in
`MohammadRefat23/MohammadRefat23.github.io`.

The project entry links to the live portfolio page. Update it if the site path
changes.
