# Visual Search Project

## 📌 Overview
This repository contains the code and notebooks for the Visual Search pipeline.  
The project processes raw satellite images, creates manifests, performs tiling, and prepares data for downstream object search.

## 📂 Repo Structure
- `notebooks/` → Jupyter/Colab notebooks for each stage  
- `metadata/` → CSV/Parquet manifests and lightweight configs  
- `src/` → (Optional) Python scripts for reusable functions  
- `data/` → **Ignored in git**, only used locally (raw/processed images)  
- `test/` → **Ignored in git**, temporary testing outputs  

## 🚀 Workflow
1. **Stage 1 - Manifest Creation**  
   - Notebook: `notebooks/01_manifest_creation.ipynb`  
   - Collect metadata from raw satellite images (dimensions, bands, stats).  

2. **Stage 2 - Preprocessing & Tiling**  
   - Notebook: `notebooks/02_preprocessing_tiling.ipynb`  
   - Splits large raw images into smaller tiles for training & analysis.  

## 🔧 Requirements
- Python 3.10+  
- Google Colab (preferred for GPU/space)  
- Key libraries: `rasterio`, `pandas`, `numpy`, `matplotlib`, `tqdm`

## 📥 Setup Instructions
1. Clone this repo:
   ```bash
   git clone https://github.com/AyushiG1026/visual_search.git
   ```
2. Place raw images under `data/raw/`
3. Run the notebooks in order (Stage 1 → Stage 2 → ...)

## 📌 Notes
- Large image files and outputs are ignored in git (`.gitignore`).  
- Use `test/` for temporary runs.  
- Share only notebooks + manifests for portability.

---
Maintainer: Ayushi Gupta  
