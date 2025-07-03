# 🧬 RNA-seq Differential Expression Analysis using `edgeR` in R

This project demonstrates a statistical RNA-seq analysis pipeline using **generalized linear modeling via `edgeR`** and **workflow management with `miodin`** in R. It builds upon an existing case–control design (LineA vs. LineB) and focuses on identifying differentially expressed genes (DEGs) from high-throughput RNA-seq data.

---

## 📌 Project Goals

- Define a reproducible RNA-seq case–control analysis design
- Filter low-count genes and normalize expression data
- Perform differential expression testing using `edgeR`
- Apply user-defined thresholds for log2 fold change and FDR
- Export and interpret top DEGs based on biological relevance

---

## 🧠 Skills Demonstrated

- RNA-seq preprocessing and statistical modeling with `edgeR`
- Workflow orchestration using `miodin`
- Outlier-aware study design reuse (Assignment 1 foundation)
- DE result filtering using `filterFDR` and `filterAbsLogFC`
- Interpretation of biological significance in top-ranked genes
- Excel-based DEG export and downstream reporting

---

## 🗂️ Project Structure

```
RNAseq-Differential-Expression-Pipeline/
├── data/
│   └── Assignment2_workspace.RData
├── results/
│   └── differential_expression_results.xlsx
├── src/
│   └── RNAseq_Differential_Expression.Rmd
```

---

## 📊 Output

The `results/` folder includes a ranked table of DEGs exported in Excel format, containing:

- **Gene symbol**
- **Log2 fold change (log2FC)**
- **Adjusted p-value (FDR)**

Top 10 genes are reported and interpreted in the R Markdown file.

---

## 📂 How to Reproduce

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/RNAseq-Differential-Expression-Pipeline.git
```

2. Open the R Markdown file in RStudio:
```R
src/RNAseq_Differential_Expression.Rmd
```

3. Load the required R packages:
```r
install.packages("miodin")
BiocManager::install(c("edgeR", "limma"))
```

4. Load the `.RData` workspace if needed:
```r
load("data/Assignment2_workspace.RData")
```

5. Run the R Markdown or knit to HTML/PDF.

---

## 👨‍💻 Author

**Fares Ibrahim**  
Bioinformatician | Systems Biology | Cancer Genomics  
🔗 [LinkedIn](https://www.linkedin.com) | 🌐 [GitHub](https://github.com/Fares77-a11y)

---

## 📄 License

MIT License – see `LICENSE` file for terms.
