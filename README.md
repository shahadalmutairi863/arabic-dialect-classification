# Arabic Dialect Classification (Senior Project)

A **final-year group project** specializing in **Arabic Natural Language Processing (NLP)**.  
The project focuses on classifying **Arabic dialects** using a combination of **classical machine learning** and **transformer-based deep learning models**.  

> 📘 *Developed as a team project for the Diploma in Data Science at the University of Jeddah.*

---

## 👥 Team Members
| Name | Student ID |
|------|-------------|
| **Shahad Almutairi** | 2315366 |
| **Ruba Alfageeh** | 2316095 |
| **Tala Melaih** | 2317013 |
| **Safaa Alsufyani** | 2315828 |

**Supervisor:** Dr. Roshayu Mohammed  
**Program:** Applied College – Diploma in Data Science  

---

## 🎯 Project Overview
Arabic dialects differ widely between regions (Najdi, Hijazi, Khaliji, Egyptian, Levantine, etc.), which makes automatic understanding difficult for NLP systems.  
This project investigates and compares different modeling techniques to automatically detect the dialect used in Arabic text.

### Objectives
- Build an NLP system that recognizes Arabic dialects.
- Compare **Logistic Regression**, **AraBERT**, and **MARBERT** models.
- Analyze the impact of preprocessing and class imbalance on model performance.
- Contribute to Arabic NLP research through a clear performance comparison.

---

## 🧠 Models Used
| Model | Description |
|--------|--------------|
| **Logistic Regression (TF‑IDF)** | Baseline classical model |
| **AraBERT** | Transformer model trained on Modern Standard Arabic and news data |
| **MARBERT** | Transformer trained on dialectal Arabic tweets and social text |

---

## 📊 Dataset
**SADA 2022 Dataset** (Saudi Data and AI Authority).  
Used the following features:
- `GroundTruthText` → Arabic text input  
- `SpeakerDialect` → dialect label  

---

## 🧹 Preprocessing Pipeline
- Text normalization and diacritics removal  
- Noise removal (emojis, punctuation, English characters)  
- Stop‑word removal  
- Tokenization  
- Character repetition handling  

---

## ⚙️ Tools & Technologies
Python | Google Colab | Scikit‑learn | PyTorch | Hugging Face Transformers | Pandas | NLTK | Matplotlib | Seaborn  

---

## 📈 Results

| Model | Accuracy | Macro F1 | Macro Recall |
|--------|-----------|-----------|---------------|
| **AraBERT** | 55.7 % | 0.249 | 0.238 |
| **MARBERT** | **56.7 %** | **0.258** | **0.246** |
| Logistic Regression (weighted) | 43 % | 0.20 | 0.33 |

---

## 🔍 Key Findings
- **MARBERT** achieved the best overall performance.  
- **AraBERT** performed strongly on formal Arabic.  
- **Logistic Regression** proved valuable for balanced, interpretable baselines.  
- **Class imbalance** was a major modeling challenge.

---

## 🧩 My Contribution – Shahad Almutairi
I played a key role in the project by focusing on data exploration, preprocessing, and preparing the foundation for both text and audio modeling.

### Responsibilities
- **Exploring New Data Modalities:**  
  While our coursework focused solely on text datasets and their preprocessing methods, I proposed expanding the project toward an audio dataset. Since we had not studied audio modeling before, I independently researched and learned the specialized models used for audio processing. I then assigned each team member a specific audio model to work on, ensuring clear task distribution.

- **Dataset Understanding & EDA:**  
  Conducted an in‑depth exploratory data analysis to understand the dataset, identify class imbalance, visualize key patterns, and clarify the challenges that would influence model performance.

- **Data Preprocessing & Cleaning**  
  Designed and implemented the full preprocessing pipeline for the dataset, including cleaning, normalization, noise removal, feature preparation, and other steps required before feeding data into any model.

- **Documentation & Team Coordination:**  
  Wrote parts of the final report, including the methodology and results sections. I also documented the preprocessing steps and coordinated task distribution among team members.

### Impact
My contributions helped introduce a new direction to the project by exploring audio datasets and their dedicated models—an area not covered in our coursework. Additionally, my EDA and preprocessing work provided a solid, clean foundation for all models and guided the deeper experiments with transformer‑based approaches.

---

## 🚀 Future Work
- Data augmentation for under‑represented dialects  
- Audio‑text multimodal learning  
- Hyperparameter tuning and cross‑validation  
- Ensemble methods  
- Explainability using SHAP or LIME  

---

## 📁 Repository Structure
```bash
arabic-dialect-classification/
├── README.md
├── requirements.txt
├── .gitignore
├── notebooks/
│   ├── preprocessing_and_AraBERT.ipynb
│   ├── MARBERT.ipynb
│   └── LogisticRegression.ipynb
├── reports/
│   └── final_report.pdf
```
---

📓 Jupyter Notebook  
📒 [View Notebook](notebooks/preprocessing__and_AraBERT..ipynb)

📄 Final Report  
📎 [View Report](reports/final_report%20(1).pdf)
---

## 🏆 Acknowledgment
Special thanks to **Dr. Roshayu Mohammed** for supervision and guidance throughout the project.

---

## 📎 Reference Links
- [SADA Dataset (Kaggle)](https://www.kaggle.com/datasets/sdaiancai/sada2022/data)  
- [AraBERT Paper – LREC 2020](https://arxiv.org/abs/2003.00104)  
- [MARBERT Paper – NAACL 2021](https://arxiv.org/abs/2101.01785)

---

📍 *University of Jeddah – Applied College – Diploma in Data Science.*

