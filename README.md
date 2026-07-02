# Sampling I — Lecture Slides

Reveal.js slide decks (Quarto) for the **Sampling I** course, Bachelor's Degree in Statistics — School of Economics (UDELAR).
Translated to English from the original LaTeX/Beamer sources.

**Author:** Juan Pablo Ferreira · <juanpablo.ferreira@fcea.edu.uy>

## Structure

```
sampling-I/
├── 01-introduction.qmd
├── 02-random-sampling.qmd
├── ...                              # 15 presentations, NN-topic.qmd
├── 15-complex-estimators.qmd
├── index.qmd                        # landing page linking every deck
├── theme/
│   └── custom.scss                  # shared modern/academic theme
└── images/
    ├── logo-fcea.png                # title-slide logo (top-left)
    └── figures/<deck>/...           # figures used by each deck
```

## Presentations

| # | File | Topic |
|---|------|-------|
| 01 | `01-introduction.qmd` | Introduction to Sample Surveys |
| 02 | `02-random-sampling.qmd` | Random Sampling |
| 03 | `03-horvitz-thompson.qmd` | The Horvitz–Thompson Estimator |
| 04 | `04-bernoulli-sampling.qmd` | Bernoulli Sampling |
| 05 | `05-systematic-sampling.qmd` | Systematic Sampling |
| 06 | `06-with-replacement-designs.qmd` | With-Replacement Designs |
| 07 | `07-poisson-sampling.qmd` | Poisson Sampling |
| 08 | `08-pps-sampling.qmd` | Probability Proportional to Size (PPS) |
| 09 | `09-stratified-sampling.qmd` | Stratified Sampling |
| 10 | `10-cluster-sampling.qmd` | Cluster Sampling |
| 11 | `11-two-stage-sampling.qmd` | Two-Stage Sampling |
| 12 | `12-sample-size-determination.qmd` | Sample Size Determination |
| 13 | `13-variance-estimation.qmd` | Variance Estimation |
| 14 | `14-domain-estimation.qmd` | Introduction to Domain Estimation |
| 15 | `15-complex-estimators.qmd` | Introduction to Complex Estimators |

## Rendering

Requires [Quarto](https://quarto.org). From this folder:

```bash
# one deck
quarto render 01-introduction.qmd

# everything (decks + index)
quarto render
```

Each deck has `embed-resources: true`, so every output `.html` is a single self-contained file (slides, theme and math embedded) that works offline.

Live preview while editing:

```bash
quarto preview 01-introduction.qmd
```

## Logo

`images/logo-fcea.png` currently holds a **placeholder**. Replace that file with the
official FCEA–UDELAR logo (same name, `images/logo-fcea.png`) and re-render — nothing
else needs to change. A vertical PNG with a transparent background works best.

## Publish to GitHub Pages (optional)

```bash
quarto render            # outputs the .html files into docs/
# commit and push; then enable Pages on the branch/folder you serve
```

## Notes

- Theme colors and fonts live in `theme/custom.scss` (Fraunces for headings, Inter for body).
- All mathematics is rendered with MathJax.
- Only figures actually used in the original LaTeX were carried over.
