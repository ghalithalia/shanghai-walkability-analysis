


# 🚶‍♀️ Shanghai Walkability – 15 Minute Accessibility Analysis

This project explores how accessible essential public services are to pedestrians in Shanghai, based on the concept of the **15-minute city**. It was developed using Python, GeoPandas, and public POI (Point of Interest) data.


📅 May 2025 – Shanghai University (UTSEUS)



##  Methodology

- Used GeoPandas to process neighborhood geometries (`sh-villages.geojson`)
- Built buffers of 5, 10, and 15 minutes using average walking speed (1.31 m/s)
- Filtered relevant POIs (supermarkets, clinics, schools, etc.) from a large dataset
- Performed spatial joins to count how many POIs are accessible per village
- Computed:
  - A score per buffer (score_5min, score_10min, score_15min)
  - A global score (sum of standardized scores)




## 📄 Full Report

📥📥 [Click here to read the full project report (PDF)](./notebooks/accessibility-15min-shanghai-ghali.ipynb)


---

## ✏️ Insights

- Accessibility increases sharply from 5 → 15 minutes, revealing spatial inequalities
- The global score is useful but hides the real local proximity




### 🛠 Tools & Skills

- Python (GeoPandas, Pandas, Seaborn, Scikit-learn)
- Spatial joins & buffer analysis
- Data cleaning and mapping

