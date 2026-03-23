# 🧪 ToxSafe-Gen: Multimodal Toxicity Prediction & Manifold Mapping

**CodeCure AI Hackathon | Track A: Drug Toxicity Prediction**  
**SPIRIT'26 – IIT (BHU) Varanasi**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR-USERNAME/ToxSafe-Gen-CodeCure-SPIRIT26/blob/main/mission_impossible.ipynb)

**🔴 Click the blue Colab badge above → Upload both .zip files → Run all cells → See everything live!**

---

### 👥 The Team
- **Susmitha** (Lead) – B.Tech 1st Year CSD, GNITS (Architecture & Lead Developer)  
- **Himanshu Podwal** – M.Sc Mathematics 1st Year, IIT Gandhinagar (Statistical Methods & Manifold Analysis)

---

### 🚀 Executive Summary
ToxSafe-Gen is a high-fidelity toxicity screening prototype. Unlike standard models that only look at small datasets, our pipeline uses **Unsupervised Pre-training on 250,000 ZINC molecules** to learn "Chemical Grammar" before fine-tuning on the Tox21 assay. This hybrid approach helps the model understand not just what a molecule looks like, but how it behaves in real chemical space.

---

### ✅ 100% Deliverables Matched (Organizers Checklist)

| Required by Organizers              | Status                          |
|-------------------------------------|---------------------------------|
| GitHub Repo + README                | ✅ Complete                     |
| Working ML Model                    | ✅ XGBoost + ZINC→Tox21 Transfer |
| Feature Importance Analysis         | ✅ SHAP + Atom Highlight        |
| Visualizations                      | ✅ Interactive Chemical Space Map |
| Simple Prediction Tool/Interface    | ✅ One-click Colab Prototype    |

**Scalability & Real-world Impact**: Designed for pharma screening (Sun Pharma style). Can scale to 1M+ molecules on GPU. SAS filter ensures molecules are not just safe but actually manufacturable.

---

### 🛠 Technical Workflow (The 4-Phase Pipeline)
**Phase 1**: Unsupervised Manifold Learning (ZINC250k)  
**Phase 2**: Supervised Specialization (Tox21) – Transfer Learning  
**Phase 3**: PCA-based Dimensionality Reduction → Interactive Chemical Space Map  
**Phase 4**: Hybrid Feature Engineering (Morgan Fingerprints + logP, QED, SAS) + XGBoost (Recall-focused)

---

### 🔬 Math Behind Our Approach (What We Actually Understood)
- We used **Eigendecomposition** to reduce 2,048-dimensional chemical space into an interactive 2D Manifold (PC1 & PC2).  
- We applied **Tanimoto Coefficient** to measure how similar new molecules are to the safe ZINC space.  

This helped us visually show why some molecules are toxic outliers.

---

### 📁 Repository Structure
- `mission_impossible.ipynb` → Complete working prototype (all code + map)  
- `chemical_space_map.html` → Interactive Plotly visualization  
- `/results` → SHAP plots + Precision/Recall metrics

---

### ▶️ Live Working Prototype (Judges – Please Test!)
1. Click the **Open in Colab** badge at the top  
2. Upload `ZINC...zip` + `Tox21...zip`  
3. Click **Runtime → Run all**

**You will instantly see:**
- Beautiful Chemical Space Map (10,000+ molecules)  
- All 10 weapons activate with green checks  
- Toxicity prediction + SAS score + SHAP explanation

**This is a fully functional, interactive prototype** — exactly as required for Round 1.

---

**Built piece by piece over 3 days with regular commits**  
(You can check the commit history — every major feature was added step-by-step)

**Made with ❤️ by Susmitha + Himanshu**  
Super excited for Round 2 live demo! We can show the full interactive prototype and explain the math live 😊


