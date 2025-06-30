# 🧬 Network Analysis: Residue Alignment & Centrality Metrics

## 📁 Overview

This repository organizes and prepares network metrics—**Degree Centrality** and **Betweenness Centrality**—from Cytoscape simulations. All values are mapped to a **consensus residue numbering scheme** to allow meaningful residue-level comparisons across different structures.

---

## 🔄 Step 1: Residue Number Alignment (Manual Step)

- **Reference File:**  (use your own script or tool to do this)
  `residue_numbers_alignment_for_all_used.xlsx`  
  → Contains **aligned consensus residue numbers**, including gaps, used for all structures.

- **Input Folder:**  
  `Raw_Data/`  
  → Contains structure-specific `.xlsx` files, each with network centrality values extracted from Cytoscape.

### 📌 What you should do:
- For each Excel file in `Raw_Data/`:
  1. **Manually copy (or write a script)** the consensus aligned residue numbers from the reference file into the **first column**.
  2. Ensure all other data columns are shifted accordingly.

> 💡 You may use your own script to automate this process if needed.

---

## 📈 Step 2: Format Output for Cytoscape Analysis

- **Expected Column Format (in order):**
  1. Aligned residue number (from the reference alignment file)
  2. *(Optional placeholder or metadata)*
  3. Original residue number (from structure-specific data)
  4. Degree Centrality
  5. Betweenness Centrality

- **Run the Script - Degree_and_Betweeness_Pipeline in each folder**  

---

## 🧪 Purpose

Aligning degree and betweeness centrality values for every residue position and output a merged file for violin plots 

---