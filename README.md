
# 📊 Centrality Analysis and Figure Reproduction

This repository contains the code and data required to reproduce the **centrality-based network analysis** and generate **Figures 2, S2, and Supplementary Figure S9** for the manuscript.

---

## 📁 Folder Structure

```
Project Root/
├── Centrality_Analysis/
│   ├── No_Urea/
│   │   └── Degree_and_Betweeness_Pipeline.ipynb
│   ├── Urea/
│   │   └── Degree_and_Betweeness_Pipeline.ipynb
│   └── README.md  ← (Refer to this for input data formats)
├── Consurf_grades/
│   ├── Consurf_Scores_pre_Processing/
│   │   └── Input files in expected format
│   └── README.md (Format details)
├── Figure_2_Pipe/
├── Supp_S9_High_DC_BC/
├── Figures2_S2.ipynb           ← Run for Figures 2 and S2
├── Supplementary_Fig_S9.ipynb  ← Run for Supplementary Figure S9
└── README.md  ← (You are here)
```

---

## 🧾 Step-by-Step Instructions

### 1️⃣ Add Raw Centrality Data

Place the Excel files containing **Degree** and **Betweenness** centrality obtained from cytoscape values in:

- `Centrality_Analysis/No_Urea/`
- `Centrality_Analysis/Urea/`

👉 **Refer to the README file in `Centrality_Analysis/`** for the correct column format of these Excel files. If you do not have simualtions in Urea just leave folder blank. 

---

### 2️⃣ Run Centrality Pipelines

Execute the following notebooks:

- `Centrality_Analysis/No_Urea/Degree_and_Betweeness_Pipeline.ipynb`
- `Centrality_Analysis/Urea/Degree_and_Betweeness_Pipeline.ipynb`

These scripts will process and merge centrality data.

---

### 3️⃣ Add Consurf Grades

Place processed conservation grade files in:

- `Consurf_grades/Consurf_Scores_pre_Processing/`

👉 See `Consurf_grades/README.md` for file format and structure.

---

### 4️⃣ Generate Final Figures

To reproduce the manuscript figures, run:

- `Figures2_S2.ipynb` → Generates **Figure 2 and Figure S2**
- `Supplementary_Fig_S9.ipynb` → Generates **Supplementary Figure S9**

---

## ✅ Output

- Processed Excel files and generated figures are saved in their respective folders.
- These outputs can be used directly for manuscript submission.

---

## 📬 Contact

For questions, reach out to mithun121@gmail.com
