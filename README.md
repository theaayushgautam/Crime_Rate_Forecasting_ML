# Crime Rate Forecasting with Facebook Prophet 🔎
📝 Project Overview
This project tackles a real-world challenge: forecasting crime rates in Chicago. Using 12 years of crime data (2006–2017) and the powerful Facebook Prophet library, we analyzed trends, identified seasonal patterns, and forecasted future crime rates.

🎯 Key Highlights

📊 6 Million Rows: Processed data from the Chicago Police Department with over 6M entries.

📅 17 Years of Crime Data: Spanning 2001 to 2017, with a forecast horizon beyond 2018.

🔮 Powered by Prophet: Leveraged Facebook Prophet for time series forecasting with trends and seasonality.

🌟 Clean Data, Clean Results: Preprocessed, cleaned, and visualized massive datasets for actionable insights.

🚀 Features
Historical Trends: Analyzed how crime rates have evolved over time.
Seasonality Detection: Identified peaks and troughs in crime rates across months and years.
Future Forecasting: Projected crime rates for the next 24 months (and beyond) with confidence intervals.
Interactive Visualization: Beautiful plots showcasing trends, seasonality, and forecasts.

📌 Interesting Facts
Did you know?
Crime rates in Chicago peak during certain seasons—can you guess which one? 🌦️☀️
The project uncovered patterns like a consistent decline in crime rates since 2008.
Your laptop can survive 6M rows of data… just barely. 😅

🔧 Tech Stack
🐍 Python
📦 Pandas, Matplotlib, Seaborn
🔮 Facebook Prophet
💻 Google Colab

### 1. Project Overview:
The project focuses on forecasting crime rates in Chicago using time series analysis and Facebook Prophet.
The dataset is sourced from the Chicago Police Department's Citizen Law Enforcement Analysis and Reporting System (CLEAR), spanning 2001–2017, with the project using data from 2005–2017.

# 2. Dataset Details:
Data is divided across three CSV files for the years 2005–2007, 2008–2011, and 2012–2017.
The combined dataset contains approximately 6 million rows and 23 columns, including features like crime type, location, and arrest status.

# 3. Tools and Libraries:
The project is implemented using Google Colab, with data stored on Google Drive.
Key libraries include pandas for data manipulation, matplotlib for visualization, and Facebook Prophet for time series forecasting.

# 4. Data Preprocessing:
Steps include concatenating multiple CSV files, handling missing values, and selecting essential columns (e.g., date, primary crime type, arrest, and location description).
The date column is converted to a datetime format for accurate time-series analysis.

# 5. Exploratory Data Analysis:
Top 10 primary crime types and crime locations are identified (e.g., "theft" and "street").
Boolean filtering is used to analyze arrests based on specific crime types and locations.

# 6. Visualization:
Crime trends are visualized by plotting yearly and monthly distributions, showing a peak in 2009 and a decline thereafter.
Decorations such as titles and axis labels are added for clarity.

# 7. Model Preparation and Training:
Data is aggregated monthly and renamed to fit Prophet’s input requirements (columns ds for date and y for measurements).
The Prophet model is trained on this aggregated dataset.

# 8. Forecasting:
The trained model predicts crime rates for a future period (e.g., 24 months).
Visualization of the forecast includes observed data (black dots) and forecast trends.

# 9. Model Saving and Reuse:
The model is saved using json serialization to avoid retraining.
Predictions can be made directly using the saved model.

# 10. Key Features of Facebook Prophet:
Handles seasonal effects and missing values robustly.
Differentiates between prediction (single outcome) and forecasting (range of outcomes).


