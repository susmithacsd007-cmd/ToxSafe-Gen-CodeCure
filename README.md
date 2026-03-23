# 🧪 ToxSafe-Gen: Multimodal Toxicity Prediction & Manifold Mapping

**CodeCure AI Hackathon | Track A: Drug Toxicity Prediction**  
**SPIRIT'26 – IIT (BHU) Varanasi**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR-USERNAME/ToxSafe-Gen-CodeCure-SPIRIT26/blob/main/mission_impossible.ipynb)

**🔴 Judges — Please Test:** Click the blue badge → Upload both .zip files → **Runtime → Run all** → Everything runs automatically!

---

### 👥 The Team
- **Susmitha** – B.Tech 1st Year CSD, GNITS (Architecture & Lead Developer)  
- **Himanshu Podwal** – M.Sc Mathematics 1st Year, IIT Gandhinagar (Statistical Methods & Manifold Analysis)

---

### 🚀 Executive Summary
ToxSafe-Gen is a working prototype that pre-trains on 250,000 ZINC molecules to learn real chemistry, then fine-tunes on Tox21 to predict toxicity. The star feature is an **interactive Chemical Space Map** that visually shows safe vs risky molecules.

### ⚔️ Our 7 Winning Differentiators (vs Standard Approach)

| Feature                  | Standard Approach       | Our Framework                          |
|--------------------------|-------------------------|----------------------------------------|
| Feature Set              | Only Fingerprints       | **Hybrid** (Fingerprints + Physicochemical) |
| Optimization             | Accuracy-focused        | **Recall-focused** (no toxic drug missed) |
| Transparency             | Black Box               | **SHAP + Atom Highlight**              |
| Practicality             | Theoretical             | **SAS Filter** (Is it buildable?)      |
| Security                 | None                    | **Adversarial Robustness + PoisonGuard** |
| Interaction              | Static Results          | **Human-in-the-Loop** (Click & Delete Atom) |
| Architecture             | Single Model            | **Multimodal Fusion** (Text + Graph + 3D) + ZINC Pre-train |

---

### 📸 Prototype Preview (What You’ll See)
| Chemical Space Map (Interactive) | SHAP + Atom Highlight |
|----------------------------------|-----------------------|
| ![Chemical Space Map](chemical_space_map.png) | ![SHAP Explanation](results/shap.png) |

---

### ✅ 100% Deliverables Matched
| Required by Organizers | Status |
|------------------------|--------|
| GitHub Repo + README   | ✅ Complete |
| Working ML Model       | ✅ XGBoost + ZINC→Tox21 Transfer |
| Feature Importance     | ✅ SHAP + Atom Highlight |
| Visualizations         | ✅ Interactive Chemical Space Map |
| Simple Prediction Tool | ✅ One-click Colab Prototype |

**Real-world Impact**: Built for Sun Pharma-style screening. SAS filter ensures drugs are manufacturable.

---




