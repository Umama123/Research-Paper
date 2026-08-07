# Structured Content Archetype Clustering — ML Capstone Project

**Author:** Umama Naseer  
**Track:** Machine Learning Track (FlyRank Internship Capstone)  
**Live Paper:** [Deployed Research Paper](https://umama123.github.io/Research-Paper/) 

---

##  Project Overview
This capstone research project applies **unsupervised machine learning (K-Means Clustering)** to group unstructured search performance metrics into automated content management archetypes.

Instead of performing manual line-by-line URL audits, this machine learning pipeline categorizes thousands of URLs into automated, actionable strategy playbooks (**Protect**, **Metadata Optimization**, **Content Refresh**, and **Merge/Prune**).

---

##  Key Results & Model Performance

By clustering multi-dimensional features (`impressions`, `clicks`, `ctr`, `avg_position`), the K-Means ML model achieved a **+370% improvement in separation capability** compared to standard quantile-based heuristic rules.

| Model Approach | Silhouette Score | Evaluation |
| :--- | :--- | :--- |
| **Quantile Heuristic Baseline** | `0.0786` | Poor cluster separation |
| **K-Means Clustering ($K=4$)** | **`0.2915`** | **Optimal Cluster Separation** |

---

##  Content Action Playbook

| Cluster ID | Archetype | Dominant Metrics | Strategy Playbook |
| :--- | :--- | :--- | :--- |
| **Cluster 1** | **Hidden Gems** | Top Position (~5.5), Low CTR (~7%) | **Metadata Optimization** — Rewrite title tags & meta descriptions. |
| **Cluster 2** | **High-Intent Drivers** | Exceptionally High CTR (~81%), High Clicks | **Protect & Monitor** — Preserve URL structure & internal links. |
| **Cluster 0** | **Growth Contenders** | High Impressions, Position ~27 | **Content Refresh** — Update content, stats & search intent. |
| **Cluster 3** | **Zombie Content** | Lowest Clicks (~4.6), CTR 2% | **Merge or Prune** — Consolidate duplicate pages or prune thin content. |

---

##  Repository Structure

```text
.
├── work/
│   └── notebooks/
│       └── capstone.ipynb      # Main Colab notebook with end-to-end ML pipeline
├── submission/
│   └── paper_url.txt           # Single-line text file containing live deployed paper URL
└── README.md                   # Project documentation
