# maternal-health-SDG3.1
# 📊 Tracking Maternal Health Progress Toward SDG 3.1

## 🎯 Problem Statement
Sustainable Development Goal (SDG) 3.1 aims to reduce the global and India's **Maternal Mortality Ratio (MMR)** to less than 70 per 100,000 live births by 2030. Despite global progress, maternal health outcomes vary widely between regions and income groups. This project provides **data-driven insights** into the key indicators influencing maternal mortality using AI and machine learning.

## 🧠 Objective
- Analyze country/state-wise data on maternal health indicators.
- Predict MMR using machine learning models.
- Identify high-impact indicators for policy intervention.

## 🧰 Tools & Technologies Used
- Language- Python  
- Libraries- Pandas, Matplotlib, Scikit-learn 
- Platform- IBM Watsonx Studio (Cloud Lite services)  
- Visualization- Correlation heatmaps, line plots  
- IBM Cloud Watsonx AI Studio- Data analysis + modeling
- IBM Cloud Watsonx AI runtime
- Cloud Object Storage – Dataset hosting
- Jupiter Notebook – Python-based analysis
- Watsonx Machine Learning – Model
- ML Model- Random Forest Regressor 
- Linear Regression

## 📁 Dataset
- **Source:** [AI Kosh | Data.gov.in](https://www.data.gov.in/resource/sustainable-development-goals-nationalindicator-framework-version-31-2021)
- **Additional Data:** National Family Health Survey (NFHS)
- **Format:** `.csv`, converted from `.xls`

## 📌 Steps Followed

### 1. Data Collection & Preparation
- Imported datasets from AI Kosh and NFHS.
- Converted `.xls` to `.csv` using MS Excel.
- Cleaned missing values (NaN) and standardized formats.

### 2. Exploratory Data Analysis (EDA)
- Used **Seaborn** and **Matplotlib** to visualize:
  - Maternal Mortality trends over time
  - State-wise variations
  - Correlations between health indicators and MMR

### 3. Feature Engineering
- Selected key indicators:
  - Maternal Mortality Rate
  - Antenatal Care (4+ visits)
  - Skilled Birth Attendance
  - Institutional Deliveries
  - Adolescent Birth Rate
  - Institutional births (in the 5 years before the survey) (%)

### 4. Machine Learning
- Watsonx Machine Learning – Model
- Used **Random Forest Regressor** to predict MMR.
- Evaluated performance with R² Score and Mean Squared Error.
- Identified top influencing features via feature importance.

### 5. Results & Insights
- Strongest predictors: Antenatal care and skilled birth attendance.
- States with lower ANC/skilled attendance showed higher MMR.
- watsonx ML model explained majority of the variance in MMR (R^2 Score: 0.17570964963497138).
- Time trend shows MMR decline in states with higher antenatal care
- Correlation heatmap reveals strongest link between adolescent birth rate and high MMR
- Regression model achieves MSE < 100, meaning reasonable prediction accuracy
- Higher ANC visits are associated with lower MMR.
- States like Kerala and Tamil Nadu have low MMR and high skilled birth attendance.
- Bihar and Assam need focused improvement.
 
## 🧪 Future Enhancements
- Integrate socio-economic factors (e.g., education, poverty rate).
- Deploy as a web dashboard for policymakers using IBM Cloud.
- Build a recommendation engine for targeted maternal interventions.
- Expand the system to global scale using WHO datasets
- Add more ML models (e.g., Random Forest, XGBoost)
- Integrate with mobile platforms for real-time community-level input

## 📎 References
- [SDG Indicators](https://sdgs.un.org/goals/goal3)
- [AI Kosh Dataset](https://data.gov.in/)
- National Family Health Survey (NFHS)
Official Website: (https://rchiips.org/NFHS/)

## ✍️ Author
Pratiksha Mahajan  
Student | IBM SkillsBuild Trainee  
