# 📊 T-Test Statistical Toolkit

A Python-based statistical toolkit for performing and interpreting three common types of t-tests — built as part of the **Tools and Methods of Data Analysis** course at **SRH University Leipzig**.

---

## 👥 Group Members

| Name | Student ID |
|---|---|
| Karthik Reddy Chilkuri | 100008159 |
| Bhanu Athava | 100007267 |
| Srikar Karipe | 100008751 |
| Manthan Milankumar Pathak | 100008521 |

---

## 📌 Overview

This toolkit performs end-to-end statistical analysis for:

- **One-Sample t-Test** — Are students sleeping the recommended 8 hours per night?
- **Independent Two-Sample t-Test (Welch)** — Do students from School GP and School MS achieve different final grades?
- **Paired t-Test** — Is there a significant within-person difference between daily steps and calories burned?

Each test includes data visualisation, assumption checks, a results table, confidence intervals, and an auto-generated conclusion paragraph.

---

## 📂 Project Structure

```
T-Test/
├── HA6-1.ipynb                          # Main Jupyter Notebook (toolkit)
├── HA6.pdf                              # Report PDF
├── data/
│   ├── student_stress_sleep_screen.csv  # Dataset 1 — One-Sample
│   ├── student-mat.csv                  # Dataset 2 — Two-Sample
│   └── Health_Sleep_Statistics.csv      # Dataset 3 — Paired
└── figures/
    ├── fig1_onesample.png
    ├── fig2_twosample.png
    └── fig3_paired.png
```

---

## 📦 Requirements

```bash
pip install numpy pandas matplotlib scipy
```

All libraries are standard and available in any Anaconda or JupyterLab environment — no extra installation needed.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/PathakMan/T-Test.git
   cd T-Test
   ```

2. Place the three CSV files inside the `data/` folder (or the same directory as the notebook).

3. Open the notebook:
   ```bash
   jupyter notebook HA6-1.ipynb
   ```

4. Run all cells top to bottom. Each cell is annotated with:
   - **WHAT** — what the cell does
   - **CHANGE** — which parameters to edit to customise the output

---

## 📊 Datasets

| Test | Dataset | Source | n |
|---|---|---|---|
| One-Sample | `student_stress_sleep_screen.csv` | [Kaggle](https://www.kaggle.com/datasets/arpitabhaskar/student-stress-sleep-and-screen-time-dataset) | 150 |
| Two-Sample | `student-mat.csv` | [Kaggle](https://www.kaggle.com/datasets/dskagglemt/student-performance-data-set) | 395 |
| Paired | `Health_Sleep_Statistics.csv` | [Kaggle](https://www.kaggle.com/datasets/hanaksoy/health-and-sleep-statistics) | 100 |

---

## 📋 Results Summary

| Test | t-statistic | p-value | Decision |
|---|---|---|---|
| One-Sample (sleep vs 8h) | −11.183 | < 0.0001 | **Reject H₀** |
| Two-Sample (GP vs MS grades) | 0.956 | 0.343 | **Fail to Reject H₀** |
| Paired (steps vs calories) | 19.844 | < 0.0001 | **Reject H₀** |

---

## 📄 Report

The full analysis report (PDF) is available in the repository: [`HA6.pdf`](./HA6.pdf)

---

## 🎓 Course Info

**Subject:** Tools and Methods of Data Analysis  
**University:** SRH University Leipzig  
**Date:** May 2026
```
