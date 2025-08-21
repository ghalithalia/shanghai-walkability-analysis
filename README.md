

```markdown
# 🚶‍♀️ Shanghai Walkability – 15 Minute Accessibility Analysis

This project explores how accessible essential public services are to pedestrians in Shanghai, based on the concept of the **15-minute city**. It was developed using Python, GeoPandas, and public POI (Point of Interest) data.

📍 Author: **Thalia Ghali**  
📅 May 2025 – Shanghai University (UTSEUS)

---

## 🎯 Objective

To evaluate **how many key services** (health, education, food, culture, etc.) are reachable **within 5, 10, and 15 minutes of walking** from every neighborhood ("village") in Shanghai.

---

## 🔬 Methodology

- Used **GeoPandas** to process neighborhood geometries (`sh-villages.geojson`)
- Built **buffers of 5, 10, and 15 minutes** using average walking speed (1.31 m/s)
- Filtered relevant POIs (supermarkets, clinics, schools, etc.) from a large dataset
- Performed **spatial joins** to count how many POIs are accessible per village
- Computed:
  - A score per buffer (score_5min, score_10min, score_15min)
  - A **global score** (sum of standardized scores)

---

## 🖼️ Visual Examples

### 🔹 Accessibility within 5 minutes

![5min](./images/map_5min.png)

### 🔹 Accessibility within 10 minutes

![10min](./images/map_10min.png)

### 🔹 Accessibility within 15 minutes

![15min](./images/map_15min.png)

### 🧮 Global Walkability Score

![global](./images/global_score_map.png)

---

## 📄 Full Report

📥 [Click here to read the full PDF](./report/accessibilité-5-10-15-Ghali.pdf)

---

## ✏️ Insights

- Accessibility increases sharply from 5 → 15 minutes, revealing spatial inequalities
- The global score is useful but hides the **real local proximity**
- To go further: build a **weighted score**, or explore **access gaps by POI category**

---

### 🛠 Tools & Skills

- Python (GeoPandas, Pandas, Seaborn, Scikit-learn)
- Spatial joins & buffer analysis
- Data cleaning and mapping

---

Let me know if you'd like to access the full code, notebook, or work with me on similar data-urbanism projects ✨
