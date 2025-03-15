# Early detection of occupational stress: Enhancing workplace safety with machine learning and large language models
**📌 A Machine Learning, Deep Learning, and NLP-based Approach**  

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)  
[![Python](https://img.shields.io/badge/Made%20with-Python-blue.svg)](https://www.python.org/)  
[![Jupyter](https://img.shields.io/badge/Notebooks-Jupyter-orange.svg)](https://jupyter.org/)  
[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](#contributing)  

---

## 📖 Table of Contents  

1. [🔍 Overview](#-overview)  
2. [📂 Repository Structure](#-repository-structure)  
3. [💻 Tech Stack](#-tech-stack)  
4. [🚀 Getting Started](#-getting-started)  
5. [🔪 Usage](#-usage)  
6. [📊 Results & Key Findings](#-results--key-findings)  
7. [📌 Industry Relevance](#-industry-relevance)  
8. [📝 License](#-license)  
9. [🤝 Contributing](#-contributing)  
10. [📬 Contact](#-contact)  

---

## 🔍 Overview  

**Workplace stress** is a critical issue that impacts **employee well-being, organizational efficiency, and workplace safety**. This repository provides **cutting-edge AI solutions** for detecting, analyzing, and mitigating occupational stress using a combination of:  

✅ **Machine Learning (ML)** for stress detection models.  
✅ **Deep Learning (DL)** using advanced neural networks.  
✅ **Natural Language Processing (NLP)** to extract insights from survey data.  
✅ **Explainable AI (XAI)** for interpretability in workplace safety decisions.  
✅ **Synthetic Data Generation** to validate model generalizability.  

**Why does this matter?**  
- Stressed workers are **more prone to workplace accidents** and lower productivity.  
- Organizations spend billions annually on absenteeism and medical costs due to work-related stress.  
- Traditional stress assessments (e.g., surveys, self-reports) are slow, subjective, and lack predictive power.  

**Our AI-driven approach** automates stress detection, enhances workplace safety, and enables proactive decision-making for both **organizations** and **policymakers**.

---

## 📂 Repository Structure  

```
📦 Occupational-Stress-Safety
├── Main_results_holdout_val.ipynb      # Main results reported in paper using holdout validation 
├── explainable_ai/                     # XAI-based analysis  
│   ├── XAI_Occupational_Stress.ipynb   
│
├── SOTA_analysis/                      # State-of-the-art comparison  
│   ├── SOTA_Paper_1.ipynb  
│   ├── SOTA_Paper_2.ipynb  
│   └── ...  
│
├── domain_analysis/                    # LLM-driven analysis  
│   ├── LLM_anova_+_rfecv.ipynb  
│
├── cross-validation/                    # Model validation  
│   ├── cross-validation.ipynb  
│
├── anova/                               # ANOVA-based feature selection  
│   ├── anova.ipynb  
│
├── rfecv/                               # Recursive feature elimination  
│   ├── RFECV.ipynb  
│
├── synthetic_data_generation/           # Synthetic dataset generation  
│   ├── Synthetic_data_generation.ipynb  
│   ├── Synthetic_data_comparison.ipynb  
│
├── eda/                                 # Exploratory Data Analysis  
│   ├── EDA_Occupational_Stress.ipynb  
│
├── ablations/                           # Impact of feature selection  
│   ├── Ablation_no_RFECV.ipynb  
│   ├── Ablation_no_anova.ipynb  
│   ├── Ablation_no_zero_var.ipynb  
│
├── dataset/                             # Raw dataset  
│   ├── DIB dataset and codebook.xlsx  
│
├── synthetic_dataset/                   # Generated datasets  
│   ├── synthetic_data_tvae.csv  
│   ├── synthetic_data_gaussian_copula.csv  
│   ├── synthetic_data_ctgan.csv  
│   ├── synthetic_data_copulaGan.csv  
│
├── LICENSE                              # MIT License  
└── README.md                            # This file  
```

---

## 💻 Tech Stack  

| Technology       | Usage |  
|-----------------|------------------------------------------------|  
| **Python**      | Core programming language |  
| **Jupyter**     | Interactive computing environment |  
| **Pandas**      | Data manipulation |  
| **NumPy**       | Numerical computing |  
| **Scikit-learn**| Machine learning models & evaluation |  
| **PyTorch**  | Deep learning framework |  
| **Hugging Face Transformers** | NLP and Large Language Models |  
| **Seaborn & Matplotlib** | Data visualization |  
| **SHAP & LIME** | Explainable AI (XAI) |  

---

## 🚀 Getting Started  

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/junayed-hasan/occupational-stress-ml.git
   cd Occupational-Stress-Safety
   ```

2. **Create a Virtual Environment**  
   ```bash
   python -m venv venv
   source venv/bin/activate  # Mac/Linux
   .\venv\Scripts\activate   # Windows
   ```

3. **Install Dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

4. **Run Jupyter Notebooks**  
   ```bash
   jupyter notebook
   ```

---

## 🔪 Usage  

### **1️⃣ Data Preprocessing & EDA**  
   - Run `eda/EDA_Occupational_Stress.ipynb` to explore dataset characteristics.  

### **2️⃣ Feature Selection & Model Training**  
   - `anova/anova.ipynb` for ANOVA-based feature selection.  
   - `rfecv/RFECV.ipynb` for recursive feature elimination.  
   - `cross-validation/cross-validation.ipynb` to validate models.  

### **3️⃣ Synthetic Data Generation**  
   - Run `synthetic_data_generation/Synthetic_data_generation.ipynb` to generate synthetic datasets.  

### **4️⃣ Explainability & Domain Analysis**  
   - `explainable_ai/XAI_Occupational_Stress.ipynb` provides model interpretability.  
   - `domain_analysis/LLM_anova_+_rfecv.ipynb` utilizes NLP models for deeper insights.  

---

## 📊 Results & Key Findings  

- **📌 Achieved 90.32% Accuracy** in occupational stress classification.  
- **📌 Top predictors of stress:** Workload, Manager Support, Job Role Clarity.  
- **📌 LLMs outperformed traditional NLP models in stress classification tasks.**  
- **📌 Synthetic data generation proved effective, achieving ~89% accuracy on unseen test scenarios.**  

For full details, check:
- `Main_results_holdout_val.ipynb` (final results)  
- `ablations/` (impact of feature selection methods)  

---

## 📌 Industry Relevance  

This research has **direct implications** for:  
✔ **HR & Workforce Management** – Predict stress & reduce workplace accidents.  
✔ **Occupational Health & Safety Teams** – Implement AI-driven monitoring.  
✔ **Government & Policymakers** – Set data-driven workplace safety regulations.  
✔ **AI & Data Science Practitioners** – Develop real-world stress detection models.  

---

## 📝 License  

This project is licensed under the [MIT License](LICENSE), allowing free use, modification, and distribution.

---

## 🤝 Contributing  

Contributions are welcome! To contribute:  
1. Fork the repository.  
2. Create a new branch (`feature-new-feature`).  
3. Commit changes and open a pull request.  

---

## 📬 Contact  

📌 **Collaborators:** Mohammad Junayed Hasan and Jannat Sultana

📌 **Supervisors:** Dr. Sifat Momen (sifat.momen@northsouth.edu, https://scholar.google.com/citations?user=sGVZEaAAAAAJ), Ms. Silvia Ahmed (silvia.ahmed@northsouth.edu, https://scholar.google.com/citations?user=T5jK--YAAAAJ&hl=en&oi=ao)

📌 **Emails:** junayedhasan100@gmail.com, jannatsultana187@gmail.com

📌 **LinkedIn:** https://www.linkedin.com/in/mjhasan21/, https://www.linkedin.com/in/jannat-sultana/

We appreciate your interest in our research and welcome discussions, collaborations, and feedback! 🚀
