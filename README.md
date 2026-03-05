## **PCOS Granulosa Cell Differential Gene Expression Analysis**

### **Overview**
This project investigates gene expression differences between granulosa cells from PCOS patients and healthy controls. It covers preprocessing, PCA‑based exploratory analysis, differential expression testing, and volcano‑plot visualization of significant genes.

### **Dataset**
- **GEO Accession:** GSE294074  
- **Raw Data:** Individual sample expression files downloaded manually

### **Folder Structure**
- `data/raw/` — raw per‑sample expression files  
- `data/processed/` — combined expression matrix  
- `notebooks/` — preprocessing and analysis notebooks  
- `results/` — plots and DEG tables  
- `README.md` — project documentation  
- `requirements.txt` — Python dependencies  

### **Workflow**
- **Preprocessing** — merge TPM values into a unified expression matrix (`expr.csv`) and fill missing values.  
- **Exploratory Analysis** — PCA to assess clustering between PCOS and control samples.  
- **Differential Expression** — t‑tests to identify DEGs and volcano plot visualization of significant and suggestive genes.

### **Usage**
1. Open notebooks in `notebooks/`.  
2. Run `01_preprocessing.ipynb` to generate `expr.csv`.  
3. Run `02_analysis_visualization.ipynb` for PCA, DEG analysis, volcano plot, and output tables.

### **Requirements**
Install dependencies with:

```bash
pip install -r requirements.txt
```
