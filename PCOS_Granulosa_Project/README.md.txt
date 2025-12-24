# PCOS Granulosa Cell Differential Gene Expression Analysis

## Overview
This project analyzes gene expression differences between granulosa cells from PCOS patients and controls. It includes preprocessing, PCA, differential gene expression analysis and volcano plot visualization.

## Dataset
- GEO accession: [GSE294074](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE294074)
- Raw data: individual sample files downloaded manually

## Folder Structure
- `data/raw/` – raw per-sample expression files
- `data/processed/` – combined expression matrix
- `notebooks/` – preprocessing and analysis notebooks
- `results/` – plots and tables
- `README.md` – this file
- `requirements.txt` – Python dependencies

## Workflow
1. **Preprocessing**  
   - Combine TPM values from each sample into a single expression matrix (`expr.csv`)  
   - Fill missing values with 0

2. **Exploratory Analysis**  
   - PCA to visualize sample clustering  

3. **Differential Gene Expression**  
   - T-tests between PCOS and control samples  
   - Volcano plot highlighting significant and suggestive DEGs  

4. **Metabolic Relevance Annotation**  
   - Annotate top DEGs for involvement in steroidogenesis, lipid, and glucose metabolism  

## Usage
1. Open the notebooks in `notebooks/`.  
2. Run `01_preprocessing.ipynb` to generate `expr.csv`.  
3. Run `02_analysis_visualization.ipynb` for PCA, DE analysis, volcano plot, and DEG table.

## Requirements
Install dependencies via:

```bash
pip install -r requirements.txt
