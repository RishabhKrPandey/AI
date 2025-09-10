# 🚢 End-to-End Exploratory Data Analysis (EDA) on the Titanic Dataset

## 📌 Project Objective
Perform a comprehensive, step-by-step exploratory data analysis to understand the key factors that influenced survival on the Titanic.

---

## 🔎 Dataset Overview

**Interpretation of `.info()`:**
- The dataset contains **891 entries (passengers)** and **12 columns**.
- **Missing Values Identified:**  
  - `Age`, `Cabin`, and `Embarked` have missing values.  
  - `Cabin` is missing ~77% of values, requiring special attention.

**Interpretation of `.describe()`:**
- **Survived:** About **38.4%** of passengers in this dataset survived.  
- **Age:** Ranges from ~5 months to 80 years, with an **average of ~30 years**.  
- **Fare:** Highly skewed — mean of **$32**, median of **$14.45**, and a max fare of **$512+**, showing extreme outliers.

📷 *Add dataset info/describe image here*

---

## 🛠️ Handling Missing Values

- For **missing values**, perform **imputation**.  
- For **skewed numerical data** → use **mean** or **median**.  
- For **categorical data** → use **mode**.  
- If a feature has **too many missing values** → either **drop it** or apply **feature engineering**.

📷 *Add missing values visualization here*

---

## 📊 Key Insights (Categorical Features)

- **Survival:** Most passengers (over 500) did **not survive**.  
- **Pclass:** The **3rd class** was the most populated, followed by 1st and then 2nd.  
- **Sex:** There were significantly more **males** than females.  
- **Embarked:** Majority embarked from **Southampton ('S')**.  
- **SibSp & Parch:** Most passengers traveled **alone**.

📷 *Add categorical plots here*

---

## 📈 Key Insights (Numerical Features)

- **Age:** Distribution peaks around the **20–30 range**.  
  - Missing values were filled with the median (**28**).  
- **Fare:** Distribution is **heavily right-skewed**, with most tickets cheap but a few very expensive ones.

📷 *Add numerical plots here*

---

## 🔗 Key Insights (Bivariate Relationships)

- **Pclass:** Clear trend →  
  - 1st class survival rate **>60%**  
  - 3rd class survival rate **<25%**  
- **Sex:** Strongest predictor →  
  - Females: **~75% survival rate**  
  - Males: **<20% survival rate**  
- **Embarked:** Passengers from **Cherbourg ('C')** had higher survival rates.  
- **Has_Cabin:** Passengers with a **cabin** had much higher survival — correlated with **1st class**.

📷 *Add bivariate plots here*

---

## 👶 Key Insight (Age vs. Survival)

- **Infants and young children** had higher survival probability.  
- A large portion of **non-survivors were young adults (20–40)**.  
- The **oldest passenger (80 years)** did not survive.

📷 *Add age vs survival plot here*

---

## 👨‍👩‍👧 Family-Size Based Insights

- Passengers who were **alone** (`IsAlone=1`) had a **lower survival rate (~30%)**.  
- **Small families (2–4 members)** had the **highest survival rate**.  
- **Large families (5+)** had very poor survival rates — likely harder to stay together during evacuation.

📷 *Add family size vs survival plot here*

---

## 🎻 Insight from Violin Plot

- **Males:**  
  - Survivors peaked at **very young ages (children)**.  
  - Non-survivors peaked in the **20–30 age range**.  

- **Females:**  
  - Distribution of survivors was **much broader**, indicating females of **most ages** had good survival chances.

📷 *Add violin plot here*

---

## 🏁 Final Conclusion and Summary of Insights

This end-to-end **EDA** has provided a deep understanding of the Titanic dataset.  
Our analysis confirms the **"women and children first"** narrative and highlights stark **social inequalities** of the time.  
Through **feature engineering**, we’ve created even more powerful predictors for a future machine learning model.

**Key Findings:**
1. **Strongest Predictors of Survival**
   - **Sex:** Being **female** was the single most significant advantage.  
     Young boys (**'Master'**) also had much higher survival rates than adult men (**'Mr'**).  
   - **Passenger Class:** Clear hierarchy → **1st > 2nd > 3rd class**.  
   - **Age:** **Children and infants** had higher survival rates.

2. **Other Influential Factors**
   - **Family Size:** **Small families (2–4)** increased survival chances.  
     Being **alone** or in **large families** reduced survival chances.  
   - **Fare / Cabin:** Having a **cabin** (higher fare) strongly correlated with survival — proxy for **wealth/class**.  
   - **Port of Embarkation:** Passengers from **Cherbourg ('C')** had higher survival, likely due to more **1st class travelers**.

<img width="846" height="650" alt="image" src="https://github.com/user-attachments/assets/9b5f038b-c35b-425c-9ac9-aa9600e3b5b3" />


---



