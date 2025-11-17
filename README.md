ENTPD1_ML: Machine Learning for Prognosis in People Living with HTLV
This repository contains Python scripts for implementing various Machine Learning models aimed at predicting prognosis in People Living with HTLV.

Project Structure
The project is initially divided into four main scripts:
- Exploratory Data Analysis (EDA): Initial data exploration and preprocessing.
- Model Selection and Optimization: Defining and optimizing machine learning models.
- Model Performance Evaluation: Assessing the predictive capability of the models.
- Explainable AI (XAI) Application: Applying XAI techniques to interpret the model's predictions.


Notes & Reminders
Clinical data has been excluded since it is yet to be extracted from medical records.
Once available, oligosymptomatic patients will be classified separately to enhance model performance.
Environment & Dependencies
The code was developed using the following versions:


Python version: 3.11.7
  
Libraries:  
- scikit-learn: 1.2.2  
- imbalanced-learn: 0.12.1  
- scikit-optimize: 0.10.1
  
Dataset Information:
The dataset used is named "cat2_df_clinic_ENTPD1.csv"

Data Dictionary:

Categorical Variables
- SEX (Sexo)
0 = Male
1 = Female

- P-HAM/TSP (PROVAVEL_HAM/TSP)
0 = No myelopathy
1 = P-HAM/TSP

- Expression_CD39_Diplotypes
3 = Genotypes associated with high CD39 expression
2 = Genotypes associated with moderate CD39 expression
1 = Genotypes associated with low CD39 expression
  - Based on association between expression levels at:
    - rs10748643 identified by MONCRIEFFE et al., 2013
      (https://doi.org/10.4049/jimmunol.190.Supp.175.4)
      
    - rs11188513 identified by WU et al., 2020
      (https://doi.org/10.2147/OTT.S272553)

- Age (Idade_clinica) = Patient's age in years.

- Binary Clinical Symptoms (0 = Absence / 1 = Presence)

- Dermatologic symtomps (Dermatológicos)
1 = Presence of dermatologic problems
0 = Absence of dermatologic problems
  
- Arthralgia (Artralgia)
1 = Presence of arthralgia
0 = Absence of arthralgia
  
- Urinary function impairment (Comprometimento da função urinária)
1 = Presence of urinary symptoms
0 = Absence of urinary symptoms
   
- Lower limb pain (Dor MMII)
1 = Presence of lower limb pain
0 = Absence of lower limb pain
  
- Limbs paresis or weakness (Paresia/ Fraqueza)
1 = Presence of paresthesia or paresis/weakness in the lower limbs
0 = Absence of paresthesia or paresis/weakness in the lower limbs
  
- Low back pain (Dor lombar/Coluna)
1 = Presence of low back pain
0 = Absence of low back pain
   
- Motor Function 
1 = Presence of motor function impairment
0 = Absence of motor function impairment

- Parestesia (Paresthesia)
1 = Presence of paresthesia
0 = Abscense of paresthesia
