# Bike Sharing Demand Forecasting & Business Decision Support

## Project Overview
Bike-sharing companies often face a mismatch between bike availability and customer demand. While some locations experience shortages, others have unused bikes. This project investigates whether better demand forecasting and bike redistribution can improve operations before investing in additional bikes.

## Business Objectives
- Analyze historical bike rental patterns and identify demand drivers.
- Perform data quality checks and exploratory data analysis (EDA).
- Formulate and statistically test a business hypothesis.
- Predict hourly bike rental demand using machine learning.
- Build a natural-language prototype for operational decision support.

## Data Analysis & Feature Engineering
Analyzed **17,379 hourly rental records** from 2011–2012. Performed data validation, identified 165 missing hourly timestamps and engineered time-based, weather-related and calendar features.

Key insights revealed higher demand during working-day rush hours, seasonal variations and lower rentals during adverse weather conditions.

## Hypothesis Testing
Applied the **Mann–Whitney U test** to examine whether working days have sharper demand peaks than non-working days.

- Working-day peak-to-average ratio: 2.96
- Non-working-day ratio: 2.30
- p-value: 6.6 × 10⁻⁷⁹

The results showed statistically significant differences in demand patterns.

## Machine Learning Model
Developed a **Random Forest Regression** model using chronological train-test splitting.

| Metric | Result |
|---|---:|
| R² Score | 0.90 |
| MAE | 45.09 |
| RMSE | 69.57 |

Achieved approximately **53% lower prediction error** compared with the historical-average baseline.

## Business Recommendation
Developed a natural-language prototype allowing operations managers to explore hourly demand, weather scenarios and peak hours.

Recommended **demand-based bike redistribution before selective fleet expansion**, supported by a four-week operational pilot measuring failed rentals, customer complaints, dock-full events and operating costs.

## Tech Stack
**Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy, Scikit-learn, Random Forest Regression, Statistical Hypothesis Testing**

## Conclusion
The project demonstrates how data analytics, statistical testing and predictive modelling can transform operational data into actionable business decisions and improve resource allocation.
