# 🔍 LIME vs SHAP: Explainability for Tabular Machine Learning

[![Python](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![XAI](https://img.shields.io/badge/topic-Explainable%20AI-orange.svg)]()

This project compares two popular post-hoc explainability methods — **LIME** and **SHAP** — on a Random Forest classifier
trained on the Breast Cancer dataset. It is designed as a mini research project for an advanced AI/ML course.

## 📁 Project Structure

```bash
.
├── README.md
├── LICENSE
├── notebooks/
│   └── xai_comparison.ipynb
├── slides/
│   └── slides_explainability_dark_gradient.pdf
├── images/
│   ├── shap_summary.png
│   └── lime_explanation.png
├── app/
│   └── gradio_xai_app.py
└── docs/
    ├── PRESENTER_SCRIPT.md
    └── YOUTUBE_NOTES.md
```

## 🚀 Getting Started

### 1. Install Dependencies

\`\`\`bash
pip install shap lime scikit-learn pandas matplotlib seaborn gradio
\`\`\`

### 2. Run the Notebook

\`\`\`bash
jupyter notebook notebooks/xai_comparison.ipynb
\`\`\`

### 3. Launch the Gradio App

\`\`\`bash
python app/gradio_xai_app.py
\`\`\`

## 📊 Methods Compared

### ✔ LIME (Local Interpretable Model-Agnostic Explanations)
- Local surrogate model around an individual prediction.
- Pros: fast, model-agnostic, intuitive.
- Cons: sensitive to sampling; not a global view.

### ✔ SHAP (SHapley Additive exPlanations)
- Based on Shapley values from cooperative game theory.
- Pros: strong theoretical grounding, global + local interpretability.
- Cons: more computationally expensive.

## 🎥 Demo Video

A short pre-recorded demo walks through:

1. Training the model  
2. Viewing a LIME explanation for a test instance  
3. Inspecting SHAP summary plot and local force plot  
4. Using the Gradio app to explore SHAP feature contributions  

👉 **YouTube link (insert here before submission).**

## 📚 References

- Ribeiro, M. T., Singh, S., & Guestrin, C. (2016). *\"Why Should I Trust You?\" Explaining the Predictions of Any Classifier.* KDD.  
- Lundberg, S. M., & Lee, S.-I. (2017). *A Unified Approach to Interpreting Model Predictions.* NIPS.  
- SHAP documentation: https://shap.readthedocs.io  
- LIME documentation: https://github.com/marcotcr/lime  
