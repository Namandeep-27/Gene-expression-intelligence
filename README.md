# 🧬 Gene Expression Intelligence Copilot  

### Turn raw gene expression datasets into structured biomarker insights — in minutes.

A modern **bioinformatics analysis platform** that transforms messy transcriptomic datasets into interpretable scientific signals using statistics, machine learning, network biology, and pathway intelligence.

Built as an interactive web application using **Python + Streamlit**, the system enables researchers to move from raw expression matrices to prioritized biological hypotheses in one seamless workflow.

---

## 🚀 Platform Overview  

![Overview](images/11.png)

This screen provides the **first high-level understanding of the dataset**, including:

- Number of samples and genes detected  
- Missing data validation  
- Number of significantly altered genes  
- Early biological signal strength indicators  
- Automatic preprocessing decisions such as log transformation and filtering  

This helps researchers quickly determine whether the dataset contains meaningful biological variation.

---

## 📊 Dataset Snapshot & Quality Summary  

![Snapshot](images/2.png)

The platform automatically identifies:

- Biological groups present in the dataset  
- Sample distribution across groups  
- Number of genes retained after cleaning and filtering  
- Key insights on how strong the tumor vs normal signal appears  

Warnings are generated when too many genes show significance, helping prevent **false discoveries caused by noisy thresholds.**

---

## 🔬 Data Health Diagnostics  

![Data Health](images/3.png)

Before performing statistical testing, the system evaluates:

- Distribution of gene expression across samples  
- Variance structure across genes  
- Potential outliers or abnormal samples  

This ensures downstream modeling and biomarker discovery are **based on reliable input data.**

---

## 📈 Differential Expression Discovery  

![Volcano Plot](images/4.png)

Each gene is tested using:

- Welch’s t-test  
- Benjamini-Hochberg FDR correction  
- Combined statistical and biological thresholds  

Interactive volcano plots allow researchers to quickly identify:

- Strongly upregulated tumor genes  
- Strongly downregulated genes  
- High-confidence biomarker candidates  

---

## 🧠 Biomarker Prioritization Engine  

![Biomarkers](images/5.png)

Instead of ranking genes using only p-values or fold change, the platform builds a **composite biomarker score** combining:

- Statistical significance  
- Effect size  
- Machine learning feature importance  
- Expression stability across samples  

Adjustable weight sliders allow researchers to tailor ranking logic to their specific biological question.

---

## 🧬 Pathway-Level Interpretation  

![Pathways](images/6.png)

Significant genes are mapped to curated biological pathway databases:

- KEGG  
- GO Biological Process  
- Reactome  
- WikiPathways  

This allows users to move beyond individual genes and understand:

> Which biological systems and mechanisms are being disrupted.

---

## 🧩 Gene Co-expression Network  

![Network](images/7.png)

Correlation-based gene networks reveal:

- Hub regulatory genes  
- Functional gene clusters  
- Network density and topology  
- Expression-driven interaction structure  

Highly connected genes may represent **master regulators worth experimental validation.**

---

## 🤖 Machine Learning Signal Validation  

The platform evaluates predictive biological signal using:

- Random Forest (primary classifier)  
- Logistic Regression  
- Support Vector Machine  
- Gradient Boosting  

Includes:

- SHAP-based feature importance  
- ROC AUC with confidence intervals  
- Automatic overfitting detection  

This helps confirm whether expression changes are **predictive, not just statistically significant.**

---

## ⏳ Survival Modeling  

When clinical metadata is available, the system performs:

- Kaplan-Meier survival stratification  
- Log-rank testing  
- Hazard ratio estimation  

This enables exploration of potential **prognostic biomarkers.**

---

## 🧬 Data Ingestion  

Supports:

- CSV / TSV / TXT  
- Excel files  
- GEO series matrix  
- Direct GEO accession loading  

Built-in datasets include:

- Cervical cancer  
- Breast cancer  
- Lung cancer  

Automatic capabilities:

- Gene column detection  
- Sample metadata inference  
- Log transformation detection  
- Data quality validation  

---

## 📊 Visualization Suite  

Includes 15+ interactive scientific charts:

- PCA clustering  
- Volcano plots  
- Heatmaps  
- ROC curves  
- Confusion matrices  
- Biomarker radar charts  
- Co-expression networks  
- Kaplan-Meier survival curves  

---

## 📤 Export Options  

- CSV biomarker tables  
- Markdown research reports  
- JSON analysis artifacts  
- PDF formatted summaries  

---

## 🏗️ Project Structure  

```bash
app.py

src/
  data_loader.py
  preprocessing.py
  differential_expression.py
  modeling.py
  biomarker_prioritization.py
  gene_network.py
  survival.py
  enrichment.py
  gene_annotation.py
  gene_info.py
  visualization.py
  ai_copilot.py
  report_generator.py
  ui_components.py
```

---

## ⚙️ Tech Stack  

**Core**
- Python  
- Streamlit  
- Pandas  
- NumPy  

**Statistics**
- SciPy  
- Statsmodels  

**Machine Learning**
- Scikit-learn  
- SHAP  

**Bioinformatics**
- Lifelines  
- NetworkX  
- Enrichr API  

**Visualization**
- Plotly  
- Matplotlib  
- Seaborn  

**AI**
- OpenAI GPT (optional)

