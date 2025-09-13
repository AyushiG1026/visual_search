# Visual Search

Content-based visual search pipeline for satellite imagery.

## Structure
- `data/raw/` — raw satellite images (NOT in Git, kept only in Google Drive)
- `data/annotations/` — JSON annotations (NOT in Git, kept only in Google Drive)
- `data/processed/` — processed tiles (NOT in Git)
- `scripts/` — Python scripts for preprocessing, encoding, etc.
- `notebooks/` — Colab notebooks for experiments

## Notes
- Large data stays in Google Drive, excluded by .gitignore.
- Only scripts, configs, and notebooks are pushed to GitHub.
