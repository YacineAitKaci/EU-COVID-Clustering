# Hierarchical Clustering for COVID-19 Impact Analysis

## 📋 Project Overview
This project applies **Hierarchical Clustering** to analyze the impact of COVID-19 across European countries. By clustering nations based on reported cases and deaths, we identify groups with similar pandemic experiences, aiding in understanding virus spread patterns.

## 🗂 Dataset
- The dataset, `data-Clustering_Hierarchique.csv`, contains **daily reported cases and deaths** across EU countries.
- **Main features:**
  - `countriesAndTerritories`: Country names
  - `cases`: Daily reported cases
  - `deaths`: Daily reported deaths
  - `popData2020`: Population in 2020
- **Size:** 28,729 rows, 11 columns
- **Preprocessing:**
  - Removed negative and missing values.
  - Aggregated data by country.
  - Standardized incidence and mortality rates.

## 🏗 Methodology
1. **Data Cleaning**: Eliminated anomalies and handled missing values.
2. **Feature Engineering**: Computed incidence and mortality rates.
3. **Standardization**: Scaled features to ensure fair clustering.
4. **Clustering Approach**:
   - Computed distance matrix using **Euclidean distance**.
   - Applied **Ward’s method** for hierarchical clustering.
   - Used a **dendrogram** to determine the optimal number of clusters.
5. **Cluster Formation**: Divided countries into **4 clusters** based on COVID-19 impact.

## 📊 Results & Visualization
- Generated **dendrograms** to visualize hierarchical relationships.
- Identified clusters grouping countries with similar COVID-19 patterns.
- Found strong correlation between **population size** and **infection impact**.

## 🔧 How to Run
1. **Install dependencies:**
```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn
```
2. **Run the clustering script:**
```bash
jupyter notebook clustering_analysis.ipynb
```

## 📌 Key Insights
- Countries like **Italy, France, and Spain** formed a high-impact cluster.
- **Smaller nations** (e.g., Iceland, Cyprus) grouped in low-impact clusters.
- The analysis helps in targeting interventions for future outbreaks.

## 🔮 Future Improvements
- Experiment with other clustering techniques (e.g., K-Means, DBSCAN).
- Incorporate additional socio-economic factors for deeper insights.
- Develop a **web-based dashboard** for interactive exploration.

---

