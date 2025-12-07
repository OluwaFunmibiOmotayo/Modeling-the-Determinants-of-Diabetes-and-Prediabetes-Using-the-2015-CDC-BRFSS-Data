# Modeling the Determinants of Diabetes and Prediabetes using Logistics and Baseline Logit Model
### Using the 2015 CDC BRFSS Data

## Project Overview
This project investigates how demographic characteristics, health behaviors, mental and
physical health status, cardiovascular comorbidities, and healthcare access
contribute to the risk of diabetes and prediabetes using the CDC's 2015 Behavioral
Risk Factor Surveillance System (BRFSS) dataset.

The goal of this project is to provide statistical insight into risk factors that may 
inform public health policy and early intervention strategies. 
---

## Data Source
- Dataset used for this project was obtaned from from Kaggle (already cleaned)
- Dataset is originally gotten from the **Behavioral Risk Factor Surveillance System (BRFSS), 2015**
- Conducted by the **Centers for Disease Control and Prevention (CDC)**
- A cross-sectional telephone survey conducted by the Centers for Disease Control and Prevention and state health departments on over 400, 000 Americans to collect data on health-related risk behaviors, chronic health conditions, and the use of preventative services. 

Key variables include:
- Diabetes status (No diabetes, Prediabetes, Diabetes)
- Sex: Sex of respondent (Male and Female)
- Age: Age category (14 categories: "18-24", "25-29", "30-34", "35-39", "40-44", "45-49", "50-54", "55-59", "60-64", "65-69", "70-74", "75-79", "80+")
- Education: Highest grade or year of school completed (6 categories: "Never attended school or only kindergarten", "Elementary", "Some high school", "High school graduate", "Some college", "College graduate")
- Income: Annual household income from all sources (8 categories: "<$10k", "$10k-$15k", "$15k-$20k", "$20k-$25k", "$25k-$35k", "$35k-$50k", "$50k-$75k", "$75k+")
- BMI: Body Mass Index
- HighBP (High blood pressure):  Told you have high blood pressure by a doctor, nurse, or other health professional (Yes/No)
- HighChol (High cholesterol):  Told by a doctor, nurse or other health professional that your blood cholesterol is high? ("No high cholesterol", "High cholesterol") 
- CholCheck: Cholesterol check in the past 5 years ("No check in 5 years", "Checked in 5 years")
- Smoker: Ever smoked at least 100 cigarettes (Yes/No) 
- GenHlth: Would you say that in general your health is "Excellent", "Very good", "Good", "Fair", "Poor")
- MentHlth: how many days during the past 30 days was your mental health not good? 
- PhysHlth: Now thinking about your physical health, which includes physical illness and injury, for how many days during the past 30 days was your physical health not good?
- DiffWalk: Do you have serious difficulty walking or climbing stairs? (Yes/No)
- Stroke: Ever told you have a stroke (Yes/No)
- HeartDiseaseorAttack: Ever reported having coronary heart disease (CHD) or myocardial infarction (MI) (Yes/No)  
- AnyHealthcare: Have any kind of health care coverage, including health insurance, prepaid plans such as HMO, etc. (Yes/No) 
- NoDocbcCost: Was there a time in the past 12 months when you needed to see a doctor but could not because of cost?  (Yes/No)
- PhysActivity: Physical activity or exercise during the past 30 days other than your regular job (Yes/No)
- Fruits: Consume fruit 1 or mor times per day (Yes/No) 
- Veggies: Consume vegetables one or more times per day (Yes/No)
- HvyAlcoholConsump: Heavy drinkers (adult men having more than 14 drinks per week and adult women having more than 7 drinks per week) (Yes/No)   
---

## Methodology
The analysis employs the following statistical approaches:
- Data cleaning and recoding of categorical predictors
- Descriptive statistics and exploratory data analysis
- Logistic and Caategory Logit models
- Model comparison using deviance and information criteria
- Interpretation of odds ratios and confidence intervals

All analyses were conducted in **R** using reproducible **R Markdown** workflows.

---

## Files in This Repository
- 'Diabetes:Prediabetes Project Slide.pdf' - Latex presentation Slide
- `Fasanya_Cat_Paper.Rmd` – RMarkdown used in generating the Journal style paper 
- `Fasanya_Cat_Paper.pdf` – Journal Style pdf report that contains Main analysis and report 
- `OluwafunmibiFinalProject.Rmd` – R code for the Analysis  
- `Diabetes:Prediabetes Project.Rproj` – RStudio project file  
- `README.md` – Project documentation  

---

## Interesting Discoveries (Summary)
- BMI impact increases sharply with age 
- Gender effect reverses with age: young men lower risk, older men higher risk than women.
- Poor physical health days increase diabetes risk only among those with very good/excellent general health.
- Having both high cholesterol and heart disease doubles the odds of diabetes.
- Physical activity does not fully offset BMI: BMI effect slightly higher in active individuals.
---

## Reproducibility
To reproduce the analysis:
1. Download the cleaned 2015 BRFSS dataset from the CDC website (attached)
2. Open the `.Rproj` file in RStudio
3. Install required R packages
4. Knit the R Markdown files

---

## Author
**Oluwafunmibi Omotayo Fasanya** 

PhD Student, Biostatistics and Data science

Louisiana State University Health Sciences Center, New Orleans 
