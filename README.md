# 🧠 Dementia Detection Using Machine Learning

## 📝 Project Overview  
This project focuses on **early-stage detection of dementia** using machine learning techniques applied to **MRI scans** and associated clinical features. Algorithms such as **SVM**, **Random Forest**, and **XGBoost** were used to classify patients into **Demented**, **Non-Demented**, and **Converted** categories with up to **80% accuracy**.

> **Highlight:** Achieved **80% classification accuracy** using SVM on clinical and MRI data from OASIS.

---

## ❓ What is Dementia?
Dementia refers to a group of symptoms affecting memory, communication, and thinking skills. It is not a specific disease, but rather a general term for cognitive impairment.  
- **Alzheimer’s disease** is the most common cause.  
- Early detection can slow disease progression and improve care planning.

---

## 🔍 Detection Modalities

Dementia can be detected using:
- 🗣 **Speech Pattern Analysis**
- 🧠 **MRI Imaging**

This project focuses on MRI analysis to detect early signs of dementia.

---

## 🧬 Dataset Details

- **Source:** [OASIS](https://www.oasis-brains.org/)
- **Subjects:** 150 right-handed individuals aged 60–96.
- **Classes:**
  - Non-Demented
  - Demented
  - Converted (later diagnosed as Demented)

### 🧾 Features Used

| Column | Description |
|--------|-------------|
| EDUC   | Years of education |
| SES    | Socioeconomic Status |
| MMSE   | Mini Mental State Examination |
| CDR    | Clinical Dementia Rating |
| eTIV   | Estimated Total Intracranial Volume |
| nWBV   | Normalized Whole Brain Volume |
| ASF    | Atlas Scaling Factor |

---

## 📊 Exploratory Analysis

### 👨‍🦳 Dementia vs Gender
| Category       | Male | Female |
|----------------|------|--------|
| Demented       | 40   | 38     |
| Non-Demented   | 22   | 50     |

### 🧠 MMSE Score
- Non-Demented group: 25–30 (higher cognitive scores)
- Demented group: Broader and lower range

### 🧠 Brain Volume (nWBV)
- Shrinking brain tissue in Demented patients leads to lower nWBV.

### 🎂 Age
- Higher prevalence of Dementia between **70–80** years.
- Lower numbers of patients above 90 suggest lower survival rate in Demented group.

---

## ⚙️ Machine Learning Models

### ✅ Random Forest
- Ensemble of decision trees
- Robust to overfitting
- Good baseline performance

### ✅ Support Vector Machine (SVM)
- Best performing model with **80% accuracy**
- Handles both linear and non-linear decision boundaries

### ✅ XGBoost
- Gradient boosting technique
- Achieved **78% accuracy**

---

## 📈 Results

- **ROC Curves** and **AUC Scores** were used for evaluation.
- **MMSE** was the most important feature.
- **Gender** and **Socioeconomic Status** had the least impact.

### 🎯 CDR Classification

| CDR Score | Meaning             |
|-----------|---------------------|
| 0         | Non-Demented        |
| 0.5       | Mild Dementia       |
| 1         | Moderate/Severe Dementia |

- SVM: **80% accuracy**  
- Random Forest: **73% accuracy**  
- XGBoost: **78% accuracy**

---

## 🔮 Future Scope

- **Multimodal Detection:** Combine MRI data with **speech analysis** for more robust models.
- **Deep Learning:** Apply CNNs and RNNs when larger datasets are available.
- **Time-Series Analysis:** Track the **progression from Converted to Demented** for better modeling.

---

## 🛠️ Technologies Used

- **Language:** Python  
- **Libraries:** Pandas, Scikit-learn, XGBoost  
- **Techniques:** Feature Importance, Classification, ROC-AUC, Ensemble Learning  
- **Dataset:** MRI & clinical data from [OASIS](https://www.oasis-brains.org/)

---

## 📌 Summary

This project demonstrates how traditional machine learning can effectively support early dementia diagnosis using MRI and clinical metadata. With further enhancement through multimodal input and larger datasets, such systems could evolve into powerful diagnostic aids in healthcare.

---

## 📎 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgements

- Dataset provided by [OASIS](https://www.oasis-brains.org/)
- Inspiration from clinical studies on Alzheimer’s and dementia detection.
