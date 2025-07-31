# Dynamic-ceRNA-Networks-Mtb
This repository contains data, scripts, and analyses from a study investigating lncRNA–miRNA–mRNA interactions that differentiate virulent (H37Rv) and avirulent (H37Ra) Mycobacterium tuberculosis infections in human macrophages, identifying key regulatory hubs and potential RNA biomarkers.

<img width="1200" height="966" alt="image" src="https://github.com/user-attachments/assets/f52f51ed-ca24-4127-8084-56a04bea0ffb" />


# 🧬 Dynamic-ceRNA-Networks-Mtb

https://static.wixstatic.com/media/6bc621_6fb4ef00f0f14e288abe54114c054a44~mv2.png/v1/fit/w_2500,h_1330,al_c/6bc621_6fb4ef00f0f14e288abe54114c054a44~mv2.png

This repository contains data, scripts, and analyses from a study investigating **lncRNA–miRNA–mRNA interactions** that differentiate virulent (H37Rv) and avirulent (H37Ra) *Mycobacterium tuberculosis* infections in **human macrophages**, identifying key regulatory hubs and potential RNA biomarkers.

---

## 📌 Overview
Tuberculosis (TB), caused by *Mycobacterium tuberculosis* (Mtb), remains a leading infectious disease worldwide. This project provides a **computational pipeline** for constructing **competing endogenous RNA (ceRNA) networks** to identify long non-coding RNAs (lncRNAs) and mRNAs that regulate host immune responses during Mtb infection.

Key features:
- Differential gene expression analysis  
- lncRNA–miRNA–mRNA interaction prediction  
- ceRNA network construction and visualization  
- Hub gene prioritization based on network centrality (MCC)  
- Functional enrichment (GO, KEGG, Reactome, WikiPathways)  
- External validation using RummaGEO datasets  
- Tissue-specific and single-cell expression profiling of biomarkers  

---


---

## 🧪 Workflow

<img width="700" alt="Graphical Abstract" src="https://github.com/user-attachments/assets/7221e91c-d1ec-4b20-b5cb-033a5c2bd697" />

This schematic shows the step-by-step approach:
1. **Data Collection:** RNA-seq dataset (GSE108731) – THP-1 macrophages infected with H37Rv and H37Ra strains over five time points (1h–48h).  
2. **Differential Expression:** Filtering of lncRNAs and mRNAs with |log2FC| ≥ 1.  
3. **Interaction Prediction:** miRNA-mediated interactions retrieved from RAID v3.0 and miRTarBase.  
4. **Network Construction:** Building ceRNA triplets and identifying high-scoring hub genes.  
5. **Functional Enrichment:** Biological processes, pathways, and tissue-specific relevance.  
6. **Validation:** Cross-dataset support using RummaGEO and ROC-AUC predictive analysis.  

---

## 📊 Key Findings
- Persistent **hub genes:** RPL30, EPC1, CSNK1D, ARID2, PPP4C, and LTBP3 emerged as central regulators across infection stages.
- Enriched pathways include **DNA damage repair**, **apoptosis regulation**, **Wnt/TGF-β signaling**, and **immune suppression**.
- Tissue-specific profiling confirmed strong expression of EPC1, CD44, RPL30, and ARID2 in **lung macrophages and immune cells**, aligning with TB pathogenesis.
- These findings provide a **framework for identifying lncRNA-regulated biomarkers** for host-directed TB therapies.

---

## ⚙️ Requirements
- Python >= 3.10  
- R >= 4.3  
- Cytoscape >= 3.10.1  
- Required packages: pandas, matplotlib, seaborn, networkx

---

## ▶️ Usage
Clone the repository:
```bash
https://github.com/IMRANINDERLOK/Dynamic-ceRNA-Networks-Mtb.git

.....


🚀 Future Directions
Experimental validation of predicted ceRNA biomarkers.

Integration with multi-omics data (proteomics, epigenomics).

Development of a web-based prediction tool for ceRNA biomarkers in infectious diseases.

