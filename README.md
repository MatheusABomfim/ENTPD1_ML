# ENTPD1_ML: Machine Learning for Prognosis in People Living with HTLV

This repository contains Python scripts that implement various machine learning models designed to prognosis people living with HTLV in terms of clinical progression to HAM/TSP.

## 📂 Project Structure

The project is initially divided into four main scripts:

1.  **Exploratory Data Analysis (EDA):** Initial data exploration and preprocessing.
2.  **Model Selection and Optimization:** Defining and optimizing machine learning models.
3.  **Model Performance Evaluation:** Assessing the predictive capability of the models.
4.  **Explainable AI (XAI) Application:** Applying XAI techniques to interpret the model's predictions.

---
## 🛠️ Environment & Dependencies

The code was developed using the following configuration:

*   **Python version:** `3.11.7`

**Key Libraries:**
```txt
scikit-learn==1.2.2
imbalanced-learn==0.12.1
scikit-optimize==0.10.1
```

---

## 📊 Dataset Information

*   **Dataset Name:** `cat2_df_clinic_ENTPD1.csv`

### Data Dictionary

#### Demographics & Status

| Variable | Original Label (PT) | Encoding / Description |
| :--- | :--- | :--- |
| **SEX** | *Sexo* | `0` = Male<br>`1` = Female |
| **Age** | *Idade_clinica* | Patient's age in years. |
| **P-HAM/TSP** | *PROVAVEL_HAM/TSP* | `0` = No myelopathy<br>`1` = P-HAM/TSP |

#### Genotypic Data: *ENTPD1* Expression

**Variable:** `Expression_CD39_Diplotypes`

*   `3` = Genotypes associated with **high** CD39 expression
*   `2` = Genotypes associated with **moderate** CD39 expression
*   `1` = Genotypes associated with **low** CD39 expression

> **References for Expression Levels:**
> Based on association between expression levels at:
> *   **rs10748643:** Identified by [MONCRIEFFE et al., 2013](https://doi.org/10.4049/jimmunol.190.Supp.175.4)
> *   **rs11188513:** Identified by [WU et al., 2020](https://doi.org/10.2147/OTT.S272553)

#### Binary Clinical Symptoms
*(Encoding: 0 = Absence, 1 = Presence)*

| Variable | Original Label (PT) | Description (Presence implies `1`) |
| :--- | :--- | :--- |
| **Dermatologic symptoms** | *Dermatológicos* | Presence of dermatologic problems |
| **Arthralgia** | *Artralgia* | Presence of arthralgia |
| **Urinary function impairment** | *Comprometimento da função urinária* | Presence of urinary symptoms |
| **Lower limb pain** | *Dor MMII* | Presence of lower limb pain |
| **Limbs paresis or weakness** | *Paresia/ Fraqueza* | Presence of paresthesia or paresis/weakness in lower limbs |
| **Low back pain** | *Dor lombar/Coluna* | Presence of low back pain |
| **Motor Function** | *Motor Function* | Presence of motor function impairment |
| **Paresthesia** | *Parestesia* | Presence of paresthesia |
