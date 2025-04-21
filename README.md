# 🌍 World Temperature Analysis App

A Streamlit web application  for exploring global temperature trends and their correlation with key environmental and socioeconomic indicators. Built using real-world data and machine learning models to uncover insights on climate change.

---

## 🔥 Why This Project Matters

Climate change is no longer a distant concern—it's a global emergency. This project dives deep into the **relationship between rising temperatures** and variables such as:

- 🌿 CO₂, methane, and nitrous oxide emissions  
- 🏙️ GDP growth and population changes  
- 🌎 Regional and seasonal temperature anomalies  

The goal? To **analyze**, **visualize**, and **predict** climate trends that shape our planet's future—using data science.

---

## 📊  Project Overview

✅ Visualizes temperature anomalies from 1960–2023  
✅ Compares seasonal trends (e.g., how winter warms faster than summer)  
✅ Highlights top CO₂-emitting countries  
✅ Shows how population growth correlates with emissions  
✅ Predicts future temperature changes using machine learning models  

---

## 🧠 Machine Learning Models

To understand and predict temperature changes, we trained and evaluated 5 models:

| Model                  | R² (Test) | RMSE  |
|-----------------------|-----------|-------|
| 📈 Linear Regression   | 0.49      | 0.46  |
| 🔁 Ridge Regression    | 0.49      | 0.46  |
| 🌳 Decision Tree       | 0.56      | 0.43  |
| 🧠 Random Forest       | **0.69**  | 0.36  |
| 🧬 Lasso Regression    | 0.47      | 0.45  |

➡️ **Random Forest Regressor** achieved the best results and was used for final insights.

---

## 🚀 Run the App Locally

You can run the app using either pip or Conda:

### 🟩 Option 1: `requirements.txt`

git clone https://github.com/aja90/world-temperature-project.git
cd world-temperature-project

pip install -r requirements.txt
streamlit run app.py


### 🟩 Option 2: environment.yaml (Conda)

git clone https://github.com/aja90/world-temperature-project.git
cd world-temperature-project

conda env create -f environment.yaml
conda activate temperature-env

streamlit run app.py


# 📈 Summary of Key Findings

## 🌡️ Global Temperature Rise: 
The project revealed a clear upward trend in global temperature anomalies over time, with a significant acceleration after 1985.

 ## ❄️ Seasonal Differences:
 Winter temperatures showed more dramatic and steeper increases compared to spring and summer, making winter the most affected season by global warming.

## 🌍 Regional Differences: 
Europe, Asia, and Africa are significantly impacted by climate change. 
Europe stands out with the most pronounced and concerning rise in temperature anomalies. The effects of climate change vary based on geographic location.

## 🔗 Correlations Between Indicators:

Very high positive correlation (0.96) between annual methane emissions and annual nitrous oxide emissions in CO₂ equivalents.

Both methane and nitrous oxide emissions are strongly correlated with population growth (0.94 and 0.90).

GDP shows a moderate correlation with methane (0.53) and nitrous oxide emissions (0.58).

Temperature anomalies have weak or negligible correlations with most other variables.

## 🏣 Top CO₂ Emitters:

UAE accounts for 27.2% of total CO₂ emissions among the top 10 countries.

Followed by Qatar (17.3%) and Equatorial Guinea (10.1%).

## 👶 Population Growth:

The global population growth rate declined from over 2.25% in the 1960s to around 1.0% by 2020.

A potential link between population growth, human activities, and climate change was observed, as population increased steadily while temperature anomalies surged after the 1970s.

## 📉 CO₂ Emissions Growth:

Emission growth rates were highly volatile in the 1960s and early 1970s.

From the 1980s onward, a steady decline occurred, reaching negative growth in recent years — possibly due to energy efficiency improvements, policies, and the COVID-19 impact.

# 🤖 Data Modeling Summary

✨ Best Performing Model:Random Forest Regressor outperformed all others with:

R² = 0.95 (Train), 0.69 (Test)

Lowest MAE, MSE, and RMSE

Detected slight overfitting, but best generalization overall

Population was the most influential feature.
