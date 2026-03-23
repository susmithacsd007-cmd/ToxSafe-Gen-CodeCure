# 🧪 ToxSafe-Gen: Multimodal Toxicity Prediction & Manifold Mapping
**CodeCure AI Hackathon | Track A: Drug Toxicity Prediction**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR-GITHUB-USERNAME/YOUR-REPO-NAME/blob/main/mission_impossible.ipynb)
*(Replace the link above with your actual Colab path)*

## 👥 The Team
* **Susmitha (Lead)** – B.Tech CSD, GNITS (Architecture & Lead Dev)
* **Himanshu Podwal** – MSc Mathematics, IIT Gandhinagar (Statistical Methods & Manifold Analysis)

---

## 🚀 Executive Summary
ToxSafe-Gen is a high-fidelity toxicity screening prototype. Unlike standard models that only look at small datasets, our pipeline uses **Unsupervised Pre-training on 250,000 ZINC molecules** to learn "Chemical Grammar" before fine-tuning on the Tox21 assay. This hybrid approach ensures the model understands not just what a molecule looks like, but how it behaves in physical space.

---

## 🛠 Technical Workflow (The 4-Phase Pipeline)

### Phase 1: Unsupervised Manifold Learning (ZINC250k)
We establish a "Baseline of Stability" using 250,000 drug-like molecules. By analyzing the global distribution of safe chemistry, the model learns to identify toxicities as statistical perturbations.

### Phase 2: Supervised Specialization (Tox21)
We perform transfer learning on the Tox21 dataset. Our model captures subtle structural deviations linked to toxicological endpoints that simpler models often miss.

### Phase 3: PCA-based Dimensionality Reduction
To visualize the high-dimensional chemical space ($R^{2048}$), we solve the **Eigendecomposition** of the feature covariance matrix. By projecting onto the primary Eigenvectors (PC1, PC2), we create an interactive **Chemical Space Universe Map**.
> **Insight:** Distance in our map equals Chemical Similarity.

### Phase 4: Hybrid Feature Engineering
We use a **Data Fusion** strategy:
* **Discrete:** 2048-bit Morgan Fingerprints (Molecular Topology).
* **Continuous:** Physicochemical Descriptors ($\log P$, QED, SAS).
* **Classifier:** XGBoost with a weighted Hessian to prioritize **Recall** (Sensitivity to Toxins).

---

## 🔬 Mathematical Foundations

### 1. The Tanimoto Similarity Metric
To measure the structural overlap between molecules:
$$T(A, B) = \frac{N_{common}}{N_A + N_B - N_{common}}$$

### 2. Interpretability via SHAP (Game Theory)
We use **Shapley Additive Explanations** to provide an "X-Ray" of our predictions. By decomposing the model's output, we can highlight the exact atoms responsible for a toxicity flag, ensuring "Human-in-the-Loop" safety.

---

## 📁 Repository Structure
* `mission_impossible.ipynb`: The core engine (Data processing $\rightarrow$ Training $\rightarrow$ Viz).
* `chemical_space_map.html`: Interactive Plotly visualization.
* `/results`: SHAP plots and performance metrics (Precision/Recall).

## ▶️ Quick Start (How to Run)
1. Click the **"Open in Colab"** badge at the top.
2. Upload the ZINC and Tox21 `.zip` datasets.
3. **Run All Cells:** The system will automatically generate the 2D Manifold and activate the Toxicity Prediction Engine.

---

