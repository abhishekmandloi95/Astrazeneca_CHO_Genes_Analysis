# Gene Marker Identification and Constitutive Gene Analysis in CHO Cells

*AstraZeneca Project*

## 📌 Project Summary

This project was conducted in collaboration with AstraZeneca to analyze RNA-seq data from CHO (Chinese Hamster Ovary) cell lines.

The project focused on two primary objectives:

1. **Gene Marker Identification** – Identify genes strongly correlated with light-chain production (`PRODUCT-TG`) that could potentially support clone selection.
2. **Constitutive Gene Characterization** – Analyze gene-expression stability and sequence characteristics across the 5'UTR, CDS, and 3'UTR regions of non-variable genes.

## 🧪 Methodology

### Gene Marker Identification

- **Data Preprocessing**
  - RNA-seq data preprocessing and normalization
  - Batch-effect correction using ComBat

- **Feature Selection**
  - Spearman correlation with `PRODUCT-TG`
  - Random Forest Regressor feature importance
  - Random Forest Classifier feature importance
  - Composite gene scoring using multiple metrics

- **Visualization**
  - Gene-expression heatmaps
  - PCA
  - t-SNE

### Constitutive Gene Analysis

- **Stability Ranking**
  - Gene-expression variance
  - Standard deviation-based stability analysis

- **Sequence Analysis**
  - Analysis of 5'UTR, CDS, and 3'UTR regions
  - DNABERT-based sequence embeddings

- **Embedding and Cluster Analysis**
  - PCA applied to DNABERT embeddings
  - Visualization of sequence-level gene distributions

## 📁 Project Structure

```text
Astrazeneca_CHO_Genes_Analysis/
├── data/                # Raw and processed RNA-seq data
├── notebooks/           # Jupyter notebooks for exploration and modelling
├── figures/             # Visualisations and feature-importance outputs
├── results/             # Final gene-ranking tables and analysis outputs
├── report/              # Final project report
├── requirements.txt     # Python dependencies
└── README.md            # Project overview and instructions
```

## 📥 Download Intermediate Outputs

Intermediate analysis files, including FIMO outputs, MEME summaries, DNABERT embeddings, and processed datasets, are available in the `v1.0` release.

```bash
wget https://github.com/abhishekmandloi95/Astrazeneca_CHO_Genes_Analysis/releases/download/v1.0/Processed_Outputs.zip
unzip Processed_Outputs.zip -d Astrazeneca_CHO_Genes_Analysis/data/processed/
```

## 📊 Tools & Technologies

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- DNABERT / Hugging Face
- MEME Suite
- FIMO
- PCA
- t-SNE
- ComBat
- Git

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/abhishekmandloi95/Astrazeneca_CHO_Genes_Analysis.git
cd Astrazeneca_CHO_Genes_Analysis
```

### 2. Install Python dependencies

```bash
pip install -r requirements.txt
```

MEME Suite and FIMO may require separate installation depending on the analysis being reproduced.

### 3. Launch the notebooks

```bash
jupyter notebook notebooks/
```

## 👨‍💻 Authors

- Abhishek Mandloi
- Amrita Moyade

This project was completed collaboratively as part of an AstraZeneca-related academic project.