# Application Documents

## LaTeX Document Register

| Document | Source | Purpose |
| --- | --- | --- |
| G-Research academic CV | `neurips2026_travel_grant/senanayak_karri_gresearch_cv.tex` | Machine-learning research profile with finance as an application domain. |
| G-Research cover letter | `neurips2026_travel_grant/cover_letter_gresearch.tex` | Supporting statement for the NeurIPS travel grant. |

## Build

Use system TeX Live and latexmk; no conda dependencies are required for these documents. See `reference_conda_env.md`.

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=/tmp/gresearch-cv neurips2026_travel_grant/senanayak_karri_gresearch_cv.tex
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=/tmp/gresearch-cv neurips2026_travel_grant/cover_letter_gresearch.tex
```
