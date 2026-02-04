# 🩺 Diabetes Health Data Analysis — Python Project

## 📘 Overview
This project explores a healthcare dataset focusing on **diabetes-related factors** such as glucose levels, BMI, blood pressure, insulin, pregnancies, and outcomes.  

The goal was to uncover trends and correlations that could help understand **patient risk patterns, clinical outcomes, and possible health interventions** — all using **Python** for data analysis and visualization.  

Through this analysis, I applied **feature engineering**, **exploratory visual analysis**, and **clinical risk grouping** to transform raw numbers into actionable insights.  

---

## 🧰 Tools Used
- **Python 3** – programming language  
- **Jupyter Notebook** – interactive coding and analysis  
- **pandas & numpy** – data manipulation and cleaning  
- **matplotlib & seaborn** – visual exploration and plotting  
- **GitHub** – for documentation, version control, and portfolio showcase  

---

## 🧹 Step 1: Data Cleaning
Imported the `diabetes.csv` dataset and prepared it for analysis.  

- Replaced zero values in physiologically impossible columns (`Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, `BMI`) with `NaN` for accurate calculations.  
- Ensured column names were correct and ready for analysis.  

---

## 📊 Step 2: Outcome Distribution
Explored how many patients were classified as diabetic (`1`) or non-diabetic (`0`).  

- This provides a **baseline overview** of the dataset.  

---

## 📈 Step 3: Glucose Level Distribution.
Patients’ glucose levels were analysed to evaluate their distribution within the dataset.

- The histogram demonstrates a right-skewed distribution, indicating that most glucose readings cluster between 90 and 150 mg/dL, with fewer patients exhibiting extremely elevated glucose levels.
- The concentration of patients within this range suggests that a substantial portion of the population may fall within elevated metabolic risk categories, highlighting the importance of continuous glucose monitoring, early screening, and preventative healthcare interventions.

🖼️ *Visualization:*  
![Glucose Histogram](images/glucose_distribution.png)

---

## ⚖️ Step 4: BMI  and Outcomes
Visualized **BMI** for non-diabetic (0) and diabetic (1) patients

- **Normal:** BMI <25  
- **Overweight:** 25 ≤ BMI <30  
- **Obese:** BMI ≥30  

Findings:  
- The boxplot shows that diabetic patients generally had higher BMI values than non-diabetic patients. The median BMI for diabetic patients was  higher than  median BMI for non-diabetic patients.
- These results support existing research showing that higher BMI is strongly associated with increased risk of developing diabetes.


🖼️ *Visualization:*  
![BMI vs Outcome](images/BMI_vs_Outcome.png)

---

## 📈 Step 5: Glucose Levels by Diabetes Outcome
Visualized **glucose levels** for non-diabetic (0) and diabetic (1) patients:    

Findings:  
- Non-diabetic patients mostly have glucose levels below ~125 mg/dL.  
- Diabetic patients generally show higher glucose, but some overlap exists.  
- This highlights **real-world variability in glucose levels and diagnosis**, providing a clear visual understanding of risk patterns.  

🖼️ *Visualization:*  
![Glucose vs Outcome](images/glucose_vs_outcome.png)

---

## 🧩 Step 6: Clinical Risk Groups
Created a **composite clinical risk feature** based on **Diabetic Outcome**:  

- **Low Risk:** All variables normal  
- **Medium Risk:** All elevated indicators indicators but below threshold of Clinical Risk
- **High Risk:** Multiple elevated indicators and above Clinical Risk threshold

This allowed a **multi-variable analysis** of patient risk patterns and clarified which groups were more likely to be diabetic.  

🖼️ *Visualization:*  
![Risk Group vs Outcome](images/Risk_Group_vs_Outcome.png)

---

## 🖼️ Step 7: Correlation Heatmap
Generated a heatmap to visualize **inter-variable relationships**:  

- Highlighted strong correlations between **glucose and outcome**, **BMI and outcome**, and moderate correlations with blood pressure.  

🖼️ *Visualization:*  
![Correlation Heatmap](images/correlation_heatmap.png)

---

## 🧮 Step 8: Summary Tables
Calculated **percentage of diabetics** within:  

- Glucose buckets  
- BMI categories  
- Clinical risk groups  

| Feature | Observation |
|---------|------------|
| Glucose | Higher ranges have higher diabetic percentages, but pre-diabetic range still shows diagnosed cases |
| BMI | Obese category has the highest prevalence of diabetes |
| Risk Group | High-risk group most predictive, but medium risk shows early warning signs |

---

## 🧠 Step 9: Key Insights
- **Glucose is the strongest single indicator** of diabetes prevalence.  
- **BMI contributes significantly**, especially in combination with elevated glucose.  
- **Clinical Risk Grouping** reveals cumulative risk patterns not apparent from single variables.  
- **Visual analysis confirms trends**, showing how Python allows quick exploration and interpretation of complex healthcare data.  

---

## 👩🏾‍🔬 About the Author
**Nontuthuko Nsele**  
Biomedical Scientist | Aspiring Clinical Data Analyst  
Passionate about health research, data analytics, and improving patient outcomes.  
🔗 [LinkedIn](https://linkedin.com/in/nontuthuko-nsele-50173012a)
