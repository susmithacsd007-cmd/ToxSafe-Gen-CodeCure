# 🧪 ToxSafe-Gen: Multimodal Toxicity Prediction & Manifold Mapping

**CodeCure AI Hackathon | Track A: Drug Toxicity Prediction**  
**SPIRIT'26 – IIT (BHU) Varanasi**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR-USERNAME/ToxSafe-Gen-CodeCure-SPIRIT26/blob/main/mission_impossible.ipynb)

**🔴 Judges — Please Test:** Click the blue badge → Upload both .zip files → **Runtime → Run all** → Everything runs automatically!

---

### 👥 The Team
- **Susmitha** (Lead) – B.Tech 1st Year CSD, GNITS (Architecture & Lead Developer)  
- **Himanshu Podwal** – M.Sc Mathematics 1st Year, IIT Gandhinagar (Statistical Methods & Manifold Analysis)

---

### 🚀 Executive Summary
ToxSafe-Gen is a working prototype that pre-trains on 250,000 ZINC molecules to learn real chemistry, then fine-tunes on Tox21 to predict toxicity. The star feature is an **interactive Chemical Space Map** that visually shows safe vs risky molecules.

---

### 📸 Prototype Preview (What You’ll See)

| Chemical Space Map (Interactive)          | SHAP + Atom Highlight                  |
|-------------------------------------------|----------------------------------------|
| ![Chemical Space Map](chemical_space_map.png) | ![SHAP Explanation](results/shap.png) |

*(Hover on the map to see SMILES, click atoms to see toxicity drop)*

---

### ✅ 100% Deliverables Matched

| Required by Organizers           | Status |
|----------------------------------|--------|
| GitHub Repo + README             | ✅ Complete |
| Working ML Model                 | ✅ XGBoost + ZINC→Tox21 Transfer |
| Feature Importance Analysis      | ✅ SHAP + Atom Highlight |
| Visualizations                   | ✅ Interactive Chemical Space Map |
| Simple Prediction Tool           | ✅ One-click Colab Prototype |

**Real-world Impact**: Built for Sun Pharma-style screening. SAS filter ensures drugs are manufacturable.

---

### 🛠 Technical Workflow (4 Phases)
**Phase 1**: ZINC Pre-training  
**Phase 2**: Tox21 Transfer Learning  
**Phase 3**: PCA → Interactive Chemical Space Map  
**Phase 4**: Hybrid Features + Recall-focused XGBoost

---

### 🔬 Mathematical Rigor & Dimensionality Reduction
- We used **Eigendecomposition** to project 2,048 dimensions into a 2D Manifold (PC1 & PC2).  
- We used **Tanimoto Coefficient** to measure similarity with the safe ZINC space.  
- We optimized the **Recall-weighted Hessian** in XGBoost so that no toxic molecule slips through (critical for patient safety).

---

### 📁 Repository Structure
- **[mission_impossible.ipynb](./mission_impossible.ipynb)** → Full working prototype  
- **[chemical_space_map.html](./chemical_space_map.html)** → Interactive map  
- **[/results](./results)** → SHAP plots + Precision/Recall metrics

---

### ▶️ Live Working Prototype (Judges – Please Test!)
1. Click the Open in Colab badge  
2. Upload ZINC.zip + Tox21.zip  
3. Click **Runtime → Run all**

You will instantly see the map + all 10 weapons + predictions.

**This is a fully functional, interactive prototype.**

---

**Built piece by piece over 3 days with regular commits**  
(Every major feature has its own commit — feel free to check history)

**Made with ❤️ by Susmitha + Himanshu**  
Super excited for Round 2! Ready to demo live and explain the math 😊

