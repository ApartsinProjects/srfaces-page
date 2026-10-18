# Submission guide — "Manufactured Matches"

Target venue: **IEEE Transactions on Biometrics, Behavior, and Identity Science (T-BIOM)**.
Secondary: **arXiv** preprint (generic two-column).

## Artifacts in this package

| File | What it is |
|---|---|
| `tbiom/` (`tbiom.zip`) | TBIOM camera-ready source: IEEEtran `[journal]` two-column. `main.tex` + `abstract.tex` + `body.tex` + `fig1.jpg` + `fig2.jpg`. |
| `arxiv/` (`arxiv.zip`) | arXiv version: IEEEtran `[conference]` two-column, no venue branding. Same content. |
| `cover_letter.tex` / `.pdf` | Cover letter to the T-BIOM Editor-in-Chief. |
| `refs.bib` | BibTeX for all 22 references (the `.tex` uses an embedded `thebibliography`, so this is supplementary). |
| `paper.pdf` (tbiom) | Compiled TBIOM PDF (for quick review / email). |
| figures `fig1.jpg`, `fig2.jpg` | Figure 1 (pooling saturation), Figure 2 (manufactured-match montage). |

Each `.tex` compiles with two `pdflatex` passes (no BibTeX pass needed). On Overleaf, set the main
document to `main.tex` and compile.

## T-BIOM submission (ScholarOne / Manuscript Central)

1. Go to the T-BIOM author portal (`mc.manuscriptcentral.com/tbiom`) and start a new submission as a
   **Regular Paper**.
2. Manuscript: upload the compiled `tbiom/paper.pdf` as the main document, and upload the `tbiom/`
   source (`main.tex`, `abstract.tex`, `body.tex`, `fig1.jpg`, `fig2.jpg`) as the LaTeX source set, or
   the single `tbiom.zip`.
3. Cover letter: paste or upload `cover_letter.pdf`.
4. Figures: `fig1.jpg`, `fig2.jpg` (also embedded in the source).
5. Keywords: open-set face recognition, watchlist identification, low-resolution face recognition,
   face super-resolution, face restoration, generative models, biometric security.
6. Confirm the originality / no-concurrent-submission statements (already asserted in the cover letter).
7. Suggested reviewers (optional): pick from the related-work authors (super-resolution-for-recognition
   and surveillance face recognition).

Before upload, check: the PDF is two-column IEEEtran, all figures render, references resolve, author
and affiliation are correct (fill the affiliation if the "independent researcher" line should change).

## arXiv submission

1. `arxiv.zip` is a self-contained source set. On arXiv's "new submission" upload the zip.
2. Primary category: `cs.CV`; cross-list `cs.CR` (security) if desired.
3. arXiv compiles with its own TeX Live; `main.tex` is the entry point.
4. Title, abstract, and authors are taken from `main.tex` / the arXiv form.

## Overleaf

The gated project page carries an "Open in Overleaf" link that imports the bundle into a fresh
Overleaf project. A persistent shared Overleaf project (if created) is linked from the same page.

## Before you submit (final checklist)

- [ ] Affiliation line in `main.tex` / `cover_letter.tex` is correct.
- [ ] `pdflatex main; pdflatex main` produces a clean PDF with resolved `\ref`/`\cite`.
- [ ] Figures 1 and 2 appear and are legible at print size.
- [ ] References 1–22 all resolve (validated with bibtest).
- [ ] Cover letter addressed to the current Editor-in-Chief.
