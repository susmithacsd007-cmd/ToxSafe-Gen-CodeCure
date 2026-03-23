# 🧪 ToxSafe-Gen: Multimodal Toxicity Prediction & Manifold Mapping

**CodeCure AI Hackathon | Track A: Drug Toxicity Prediction**  
**SPIRIT'26 – IIT (BHU) Varanasi**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR-USERNAME/ToxSafe-Gen-CodeCure-SPIRIT26/blob/main/mission_impossible.ipynb)

**🔴 Click the blue Colab badge above → Upload both .zip files → Run all cells → Everything works live!**

---

### 👥 The Team
- **Susmitha** – B.Tech CSD, GNITS (Architecture & Lead Developer)  
- **Himanshu Podwal** – M.Sc Mathematics, IIT Gandhinagar (Statistical Methods & Manifold Analysis)

---

### 🚀 Executive Summary
ToxSafe-Gen is a high-fidelity toxicity screening prototype. Unlike standard models that only look at small datasets, our pipeline uses **Unsupervised Pre-training on 250,000 ZINC molecules** to learn "Chemical Grammar" before fine-tuning on the Tox21 assay. This hybrid approach ensures the model understands not just what a molecule looks like, but how it behaves in physical space.

---

### ✅ 100% Deliverables Matched (Organizers Checklist)

| Required by Organizers              | Status                          |
|-------------------------------------|---------------------------------|
| GitHub Repo + README                | ✅ Complete                     |
| Working ML Model                    | ✅ XGBoost + ZINC→Tox21 Transfer |
| Feature Importance Analysis         | ✅ SHAP + Atom Highlight        |
| Visualizations                      | ✅ Interactive Chemical Space Map |
| Simple Prediction Tool/Interface    | ✅ One-click Colab Prototype    |

**Scalability & Real-world Impact**: Built for pharma screening (Sun Pharma style). Can easily scale to 1M+ molecules on GPU. SAS filter ensures suggested molecules are actually manufacturable.

---

### 🛠 Technical Workflow (The 4-Phase Pipeline)

**Phase 1: Unsupervised Manifold Learning (ZINC250k)**  
Baseline of Stability using 250,000 drug-like molecules.

**Phase 2: Supervised Specialization (Tox21)**  
Transfer learning to capture toxicological endpoints.

**Phase 3: PCA-based Dimensionality Reduction**  
Eigendecomposition → Interactive **Chemical Space Universe Map**.  
*Insight: Distance in map = Chemical Similarity*

**Phase 4: Hybrid Feature Engineering**  
- Discrete: 2048-bit Morgan Fingerprints  
- Continuous: logP, QED, SAS  
- Classifier: XGBoost with weighted Hessian (prioritizes Recall)

---

### 🔬 Mathematical Foundations
1. **Tanimoto Similarity** – Structural overlap metric  
2. **SHAP (Game Theory)** – X-Ray explanation with Human-in-the-Loop atom highlighting

---

### 📁 Repository Structure
- `mission_impossible.ipynb` → Complete working prototype  
- `chemical_space_map.html` → Interactive Plotly map  
- `/results` → SHAP plots + Precision/Recall metrics

---

### ▶️ Live Working Prototype (Judges – Please Test!)

1. Click the **Open in Colab** badge at the top  
2. Upload `ZINC...zip` + `Tox21...zip`  
3. Click **Runtime → Run all**  

**What you will instantly see:**
- Beautiful Chemical Space Map (10,000+ molecules)  
- All 10 weapons activate with green checks  
- Toxicity prediction + SAS score + SHAP explanation  

**This is a fully functional, interactive prototype** — exactly as required for Round 1.

---




