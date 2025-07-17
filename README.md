
# 📊 Centrality Analysis and Figure Reproduction
This repository contains Jupyter notebooks with scripts for analyzing and visualizing residue interaction networks in apoptotic caspases. The analysis focuses on degree and betweenness centrality metrics to identify key residues involved in allosteric regulation and conformational dynamics.
The visualizations are generated using Seaborn to provide clear and interpretable insights into structural communication pathways.
This work is part of the manuscript titled “Evolution-guided centrality analysis reveals allosteric communication hotspots in apoptotic caspases”, currently under review for publication in the Biochemical Journal.
This repository contains the code and data required to document the workflow and reproduce the **centrality-based network analysis**, generate **Figures 2, S2, and Supplementary Figure S9** for the manuscript.

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

Place the Excel files containing **Degree** and **Betweenness** centrality obtained from the sensenet application (https://apps.cytoscape.org/apps/sensenet) within cytoscape (https://cytoscape.org/) using frames from MD simulations (Gromacs):

- `Centrality_Analysis/No_Urea/`
- `Centrality_Analysis/Urea/`

👉 **Refer to the README file in `Centrality_Analysis/`** for the correct column format of these Excel files. If you do not have simualtions in Urea just leave urea folder blank. 

---

### 2️⃣ Run Centrality Pipelines

Execute the following notebooks:

- `Centrality_Analysis/No_Urea/Degree_and_Betweeness_Pipeline.ipynb`
- `Centrality_Analysis/Urea/Degree_and_Betweeness_Pipeline.ipynb`

These scripts will process and merge centrality data in different sub folders.

---

### 3️⃣ Add Consurf Grades

Place processed conservation scores obtained from consurf (https://consurf.tau.ac.il/consurf_index.php) in:

- `Consurf_grades/Consurf_Scores_pre_Processing/`

👉 See `Consurf_grades/README.md` for the required formatting to successfully execute the scripts.

---

### 4️⃣ Generate Final Figures

To reproduce the manuscript figures, run:

- `Figures2_S2.ipynb` → Generates **Figure 2 and Figure S2**
- `Supplementary_Fig_S9.ipynb` → Generates **Supplementary Figure S9**


## 📬 Contact

For questions, reach out to mithun121@gmail.com
