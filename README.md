# NYC Yellow Taxi Data Analysis 🚕📊
<img width="605" height="230" alt="image" src="https://github.com/user-attachments/assets/14fdbb62-561e-4382-9c24-795b2aa3e1fb" />

---

## Overview
This project analyzes 2017 New York City Yellow Taxi trip data. The dataset includes trip distances, fares, tips, passenger counts, pickup/dropoff times, and locations. The goal is to clean and explore the data, identify patterns, and generate insights for taxi operators, analysts, and NYC TLC stakeholders.

---

## Introduction
Yellow taxis are an iconic part of New York City. They provide a convenient way for passengers to travel while relaxing or using their time productively. Understanding trip durations, fares, tipping, and peak demand areas can help drivers, passengers, and analysts make better decisions.

---
## Motivation
New York City is always busy, with heavy traffic, pedestrians, and public transit. Analyzing taxi trips can reveal patterns such as:
- Expected trip durations and distances.
- Peak demand times and locations.
- Tips, behavior, and fare distribution.
These insights improve operational efficiency, enhance passenger experience, and support predictive modeling for demand or fare forecasting.


---

## Objectives
- Clean and preprocess raw TLC trip data.  
- Explore trip distances, fares, and tipping behavior.  
- Compare vendors and payment methods.  
- Analyze passenger counts and their impact on tips.  
- Examine patterns by month and day.  
- Generate visualizations and actionable business recommendations.  

---

## What I Did (Summary)
- Converted pickup/dropoff timestamps to datetime format; created `month`, `day`, and `trip_duration`.  
- Checked for missing values, zero trips, negative fares, and other anomalies.  
- Plotted histograms and boxplots for `trip_distance`, `total_amount`, and `tip_amount`.  
- Grouped data by vendor, passenger count, day, and month to identify patterns.  
- Calculated mean trip distance per drop-off location and total revenue by day/month.  

---

## Key Insights — Part One (Trip & Fare Patterns)
- **Trip distances:** Most rides are short (median ≈ 1.6 miles; 75% ≤ 3 miles), but outliers reach 33 miles.  
- **Fares:** Median total fare ≈ $10; outliers skew the distribution up to $1,200.  
- **Tips:** Median ≈ $1; many trips show $0 tip (especially cash). Vendor 2 has more high-tip trips than Vendor 1.  
- **Passenger count vs. tip:** Single-passenger trips are most common. Tips do not increase linearly with passenger count; 5-passenger trips show unusually high tips.  

---

## Key Insights — Part Two (Time & Location Patterns)
- **Monthly demand:** Highest in March, October, and May; lowest in July, August, and September.  
- **Daily demand:** Busiest days are Thursday and Friday.  
- **Revenue trends:** Follow similar patterns — peak revenue on Thursdays and in May/October.  
- **Drop-off locations:** 216 unique IDs; a small number of locations receive most trips (likely airports, transit hubs, tourist areas).  
- **Trip duration:** Most trips are under 30 minutes; duration correlates with distance.  

---

## Business Recommendations
- Allocate drivers to high-demand areas and peak times (Thursday–Friday afternoons/evenings).  
- Consider surge or distance-based pricing for long, high-value trips.  
- Promote cashless payments to capture tips reliably (credit card trips record tips; cash often shows $0).  
- Flag anomalies (zero distance, zero passengers, negative fares) for cleanup and auditing.  
- Use `trip_distance` and `total_amount` as primary features for predictive modeling (fare or demand).  

---

## How to Run This Analysis
1. Open the included Jupyter Notebook (`NYC_Taxi_EDA.ipynb`).  
2. Ensure Python packages are installed: `pandas`, `numpy`, `matplotlib`, `seaborn`.  
3. Load the raw CSV dataset (path specified at the top of the notebook).  
4. Run the notebook cells to generate cleaned data and visualizations.
   
---

## Tools & Libraries
- Python (`pandas`, `numpy`, `matplotlib`, `seaborn`)  
- Jupyter Notebook  
- GitHub  

---



