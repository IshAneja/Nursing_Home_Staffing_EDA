# 🏥 Nursing Home Staffing EDA

## Overview 

This project explores nursing home staffing levels across facilities in the United States, with the goal of identifying key factors that impact staffing ratings and how facilities can improve their performance. Using robust data exploration and visualization techniques, this analysis uncovers insights into staffing trends, regulatory benchmarks, and the relationship between staffing inputs and quality ratings.

---

## 📌 Project Objective

- Looking at the relationship between staffing rating and nursing staff hours per resident per weekday.
- Understand the distribution and variation of nursing staff hours per resident per day.
- Identify opportunities for facilities to improve their staffing level ratings.
- Analyze the distribution of contract vs. full-time employees across states and facilities, and assess how these employment types impact overall staffing rating. 
- Present data-driven insights through compelling visualizations.
---

## 📁 Repository Structure

```bash
Nursing_Home_Staffing_EDA/
├── Nursing_Home_Staffing_EDA.ipynb               # Main notebook with EDA and Visualizations
├── Nursing_Home_Staffing_EDA.html                # HTML export for quick viewing
├── requirements.txt                              # Dependencies list
├── README.md                                     # This file
├── data/
│   ├──NH_ProviderInfo_Apr2024.csv                # Nursing home dataset April
│   ├──NH_ProviderInfo_May2024.csv                # Nursing home dataset May
│   └──NH_ProviderInfo_Jun2024.csv                # Nursing home dataset June
├── images/
│   ├── staffing_rating.png                       # Violin Plot of Staffing Ratings across providers 
│   ├── heatmap_of_staffing_levels.png            # Correlation Heatmap of Staffing Rating and Nursing Staff Hours
│   ├── multi_state_charts.png                    # Top States and Bottom States of various categories
│   ├── staffing_hours_vs_staffing_rating.png     # Scatterplot of Staffing Hours vs. Staffing Rating
│   ├── fines_vs_staffing_rating.png              # Scatterplot of Amount of Fines vs. Staffing Rating
│   ├── staffing_hours_vs_certified_beds.png      # Scatterplot of Staffing Hours vs. Number of beds
│   ├── staffing_hours_vs_residents_per_day.png   # Scatterplot of Staffing Hours vs. avg. number of Residents
│   ├── fines_vs_nursing_staff_hours.png          # Scatterplot of Amount of Fines vs. Staffing Hours
│   ├── resident_levels_by_state.png              # Bar Chart showing Number of Residents vs. Number of beds
│   ├── high_contract_worker_staffing_rating.png  # Violin Plot of High Contract worker staffing rating across providers
│   └── high_contract_staffing_state.png          # Bar Chart of high contract staffing levels accross each state
``` 

## 📊 Datasets

### This project uses two different datasets 

1. Source: Payroll Based Journal [dataset](https://data.cms.gov/quality-of-care/payroll-based-journal-daily-nurse-staffing)

    Description: Information on Payroll-Based Journal staffing submitted by long term care facilities. Data are presented as one row per work day, for each facility.

### Features used include:

- Provider Name, State, City
- Calendar Quarter
- Employee Hours for RN, LPN, CNA, and Med Aide/Technicion 
- Contract Hours for RN, LPN, CNA, and Med Aide/Technicion 

2. Source: Nursing Home Including Rehab Services [dataset](https://data.cms.gov/provider-data/topics/nursing-homes)

    Description: These datasets allow you to compare the average level of a nursing home's performance in certain areas of care for Medicare-certified skilled nursing facilities and nursing homes nationwide.

### Features used include: 

- Staffing Rating, Quality Rating
- Nurse Staffing on the Weekdays and Weekends 
- Number of fines and amount of fines paid by facilities 
- Number of beds at facilities and number of residents at facilities
---

## 🧪 Methods & Tools

- Python (Pandas) for data cleaning and analysis
- Seaborn and Matplotlib for data visualization
- Jupyter Notebook for interactive development
---

## 📊 Visualizations

- Scatter Plots comparing number of beds vs. staffing levels, colored by staffing rating
- Violin Plots to show distribution of overall rating and staffing rating 
- Heatmaps for staffing feature correlation
- Bar Charts to show number of residents and beds in each state 
---

## 🔍 Key Insights

- Facilities with larger sizes or inadequate staffing levels are more likely to experience declines in staffing ratings.
- A high reliance on contract workers, compared to full-time staff, is associated with lower staffing ratings.
- Understaffed facilities serving a high number of residents are more prone to incurring fines due to inadequate quality of care.
---
## 📈 Recommendations

- Facilities aiming to improve from a 2-star to a higher rating should prioritize increasing direct care staff coverage to above 2 hours per resident per day.
- Increasing staffing hours per resident is correlated with improved care quality and may help reduce the likelihood of penalties and citations.
- Facilities with fewer than 300 certified beds tend to maintain higher staffing adequacy, suggesting that managing facility size can contribute to better resident outcomes. 
--- 

## 📌 To-Do
- Analyze how states and facilities with a high proportion of contract workers achieve high staffing ratings.
- Examine weekday vs. weekend staffing level trends to uncover potential variability in care delivery. 
- Adding additional datasets to create a timeseries analysis. We only focused on Q2 however it would be interesting to add addtional months/years to do a month over month, quarter over quarter, year over year analysis. 
- Apply machine learning techniques such as Principal Component Analysis (PCA) and K-Means clustering identify patterns in staffing data and compare clustering results against staffing level ratings.
---

## 🛠️ Installation & Usage

1. Clone the repository:
```sh 
git clone https://github.com/IshAneja/Nursing_Home_Staffing_EDA.git
cd Nursing_Home_Staffing_EDA
```

2. Install dependencies:
```sh
pip install -r requirements.txt
```
3. Run the notebook:

Open [Nursing_Home_Staffing_EDA.ipynb](https://github.com/IshAneja/Nursing_Home_Staffing_EDA/blob/main/Nursing_Home_Staffing_EDA.ipynb) in Jupyter or VS Code.

---

👤 Author
Ish Aneja

📫 [Ish.Aneja@outlook.com](mailto:Ish.Aneja@outlook.com)
🔗 [LinkedIn](https://https://www.linkedin.com/in/ish-aneja/)
📘 [Portfolio](https://ishaneja.github.io/)

📄 License
This project is open-source under the MIT License.
