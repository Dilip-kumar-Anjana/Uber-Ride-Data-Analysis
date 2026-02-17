# 🚗 Uber Ride Data Analysis
## 📌 Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) and data preprocessing on an Uber ride dataset to identify ride patterns, travel behavior, and business insights.

📊 Dataset Description

The dataset contains:

Start & End Date

Ride Category (Business/Personal)

Start & Stop Locations

Miles Travelled

Purpose of Ride

Day Name

Time Label

Month

Duration

🛠️ Work Performed

✔ Data Cleaning
✔ Feature Engineering (Day, Month, Duration Extraction)
✔ Outlier Treatment using IQR Method
✔ Time Series Analysis (Daily Miles Trend)
✔ Data Encoding
✔ Visualization using Matplotlib

📈 Key Analysis Example

Outlier treatment using IQR method:

Q1_miles = np.percentile(df['miles'], 25)
Q3_miles = np.percentile(df['miles'], 75)
IQR_miles = Q3_miles - Q1_miles


Daily miles trend visualization:

daily_miles = df.resample('D')['miles'].sum()
plt.plot(daily_miles.index, daily_miles.values)

🎯 Skills Demonstrated

Python

Pandas

NumPy

Data Cleaning

Exploratory Data Analysis

Data Visualization

Outlier Detection

Time Series Aggregation

📌 Conclusion

The analysis helped identify ride usage trends, peak travel periods, and business ride patterns. Proper outlier handling improved dataset reliability for further modeling tasks.

👨‍💻 Author

Dilip Kumar Anjana
B.Tech CSE | Data Analytics Enthusiast
