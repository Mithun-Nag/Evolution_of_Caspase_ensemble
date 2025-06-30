# 🧬 Residue Annotation and Conservation Mapping

## 📄 Input File Format

This file annotates each residue position based on the Caspase-8 consensus numbering and provides structural and evolutionary context. It is used to integrate residue-level data for downstream analysis and manuscript figures.

Each row corresponds to a residue, with the following columns:

| Column Name            | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| `A_Cp8_Numbering`      | Residue index based on the Caspase-8 consensus alignment                    |
| `short_SS`             | Secondary structure label (e.g., loop, sheet, helix) used in the manuscript |
| `Caspase 8`            | Residue identity at this position in human Caspase-8                        |
| `Consensus`            | Most common residue across the alignment with its percentage (e.g., Y 100.000) |
| `Conservation_Score`   | Conservation score computed using **ConSurf**                               |
| `Possibilities`        | List of observed amino acids at this aligned position across homologs       |

---

## 🛠️ Output Format from Script

The script processes the input to generate a simplified file with the following columns:

| Column Name            | Description                                                       |
|------------------------|-------------------------------------------------------------------|
| `A_Cp8_Numbering`      | Aligned consensus residue number                                   |
| `short_SS`             | Secondary structure annotation                                     |
| `Conservation_Score`   | ConSurf-based conservation score                                   |
| `Conservation`         | Discrete conservation category assigned based on the score         |

---

## 🧮 Conservation Category Assignment

The `Conservation` column is derived from `Conservation_Score` using the following rules:

- **Highly Conserved**: Score **9 or 8**
- **Intermediate**: Score **7 to 5**
- **Variable**: Score **4 or below**

These labels are useful for visualizing conservation trends alongside structural or functional data.
