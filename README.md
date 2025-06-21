## 📘 Project Scenario

You are working as a data scientist for a healthcare analytics company. You have been provided with a dataset containing anonymized patient data. Your task is to clean the data, visualize trends, analyze statistical relationships, and simulate a basic health-related system using First Order ODEs.

---

## ✅ Tasks Overview

### 🔹 Q1: Outlier Detection and Feature Reduction (2 Marks)

- Applied `VarianceThreshold` to remove constant features.
- Detected and removed outliers from `CholesterolLevel` using the IQR method.
- Replaced any missing values using appropriate techniques.

### 🔹 Q2: Data Visualization (2 Marks)

- Created a **box plot** comparing `BloodPressure` across different `RiskCategory` levels.
- Generated a **count plot** showing the number of patients in each `RiskCategory` per `Region`.

### 🔹 Q3: Statistical Hypothesis Testing (3 Marks)

#### 📌 Test 1: One-Sample T-Test
- **Hypothesis:**  
  - H₀: Mean CholesterolLevel = 200  
  - H₁: Mean CholesterolLevel ≠ 200  
- Sample size: 20  
- Test statistic and p-value calculated  
- Conclusion based on p-value

#### 📌 Test 2: Chi-Square Test of Independence
- **Hypothesis:**  
  - H₀: Region and RiskCategory are independent  
  - H₁: Region and RiskCategory are associated  
- Performed using a contingency table  
- Test statistic and p-value provided  
- Interpretation based on the result

### 🔹 Q4: ODE Simulation of Drug Concentration (3 Marks)

- Modeled the equation:  
  \[
  \frac{dC}{dt} = k(D - C) \quad \text{where } k = 0.1, D = 100, C(0) = 0
  \]
- Simulated over \( t = 0 \) to \( t = 50 \)
- Used both `odeint` and `solve_ivp` from `scipy.integrate`
- Plotted both solutions and compared their outputs


