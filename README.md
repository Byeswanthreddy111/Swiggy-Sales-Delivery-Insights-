
<h1 align="center"> Swiggy Sales Delivery Insights </h1>
<img src="https://github.com/Sanskrutee-Dudhe/swiggy_Food_Delivery/assets/122347459/ac45c8cb-6dda-4e36-8182-3acd20431b53" width='900px' height='500px' >
# 🍔 Swiggy Food Delivery — Data Analysis & Dashboard

### End-to-End Data Analytics Project | Web Scraping → SQL → Power BI Dashboard

[![Python](https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Selenium](https://img.shields.io/badge/Selenium-Web%20Scraping-43B02A?style=for-the-badge&logo=selenium&logoColor=white)](https://selenium.dev)
[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![MySQL](https://img.shields.io/badge/MySQL-SQL%20Analysis-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://mysql.com)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Excel](https://img.shields.io/badge/Excel-Data%20Cleaning-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://microsoft.com/excel)

> **B.Tech Final Year Project | Computer Science & Engineering**

</div>

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Business Problem](#-business-problem)
- [Project Workflow](#-project-workflow)
- [Dashboard Preview](#-dashboard-preview)
- [Tech Stack](#️-tech-stack)
- [Data Acquisition — Web Scraping](#-data-acquisition--web-scraping)
- [Data Preprocessing](#-data-preprocessing)
- [SQL Analysis](#-sql-analysis)
- [Key Insights](#-key-insights)
- [Strategic Recommendation](#-strategic-recommendation)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Challenges & Learnings](#-challenges--learnings)
- [Future Scope](#-future-scope)

---

## 🌟 Project Overview

**Swiggy Food Delivery Analysis** is a complete end-to-end data analytics project that scrapes real restaurant data from **Swiggy** — India's leading food delivery platform — performs in-depth analysis, and delivers actionable business intelligence through an interactive **Power BI dashboard**.

The project was built to help a **consultancy firm** make a data-backed decision on **where to open a remote/cloud kitchen in Bangalore**, analyzing restaurant profiles, cuisines, pricing structures, delivery times, and customer ratings across the city.

---

## 💼 Business Problem

> *"A consultancy firm wants to open a remote kitchen in Bangalore. Where should they set it up? Which cuisines should they serve? What price point works best?"*

This project answers exactly that — using scraped data, statistical analysis, and a geospatial Power BI dashboard to identify the **optimal location, cuisine, and pricing strategy** for a new cloud kitchen in Bangalore.

---

## 🔄 Project Workflow

```
┌─────────────────────────────────────────────────────────────────────┐
│                        PROJECT PIPELINE                             │
│                                                                     │
│  ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────────┐  │
│  │  Swiggy  │───▶│   Web    │───▶│  Excel   │───▶│    MySQL     │  │
│  │ Website  │    │ Scraping │    │ Cleaning │    │  SQL Queries │  │
│  │          │    │(Selenium)│    │& Feature │    │  Analysis    │  │
│  └──────────┘    └──────────┘    │Engineering    └──────┬───────┘  │
│                                  └──────────┘           │          │
│                                                          ▼          │
│                                               ┌──────────────────┐  │
│                                               │  Power BI        │  │
│                                               │  Interactive     │  │
│                                               │  Dashboard       │  │
│                                               └──────────────────┘  │
└─────────────────────────────────────────────────────────────────────┘
```

---

## 📊 Dashboard Preview

> The Power BI dashboard (`Swiggy Dashboard.pbix`) visualizes all key metrics across Bangalore's restaurant ecosystem.

### 🗺️ Overview Dashboard — City-Wide Restaurant Intelligence
![Analytics Dashboard]<img width="800" height="522" alt="image" src="https://github.com/user-attachments/assets/419afcf2-7402-498e-98a7-b98a934271d3" />

*Interactive Power BI dashboard showing restaurant density, average ratings, price ranges, and cuisine distribution across Bangalore neighbourhoods.*

---

### 📍 Location Heatmap — High-Demand Zones in Bangalore
![Location Heatmap]<img width="800" height="459" alt="image" src="https://github.com/user-attachments/assets/defcd13e-441f-4621-a8b7-3c06d3cd478a" />

*Geographic heatmap identifying customer concentration hotspots — Koramangala, Indiranagar, and Ashok Nagar emerge as the top 3 high-demand zones.*

---

### 🍽️ Cuisine & Pricing Intelligence
![Cuisine Analysis]<img width="800" height="445" alt="image" src="https://github.com/user-attachments/assets/13859814-69a4-4dae-8324-3f9dbd445801" />

*Bar charts and treemaps breaking down the most popular cuisines, average cost for two, and price band distribution across restaurant categories in Bangalore.*

---

## ⚙️ Tech Stack

| Layer | Tool / Library | Purpose |
|---|---|---|
| **Web Scraping** | Python, Selenium, BeautifulSoup | Automated data extraction from Swiggy |
| **Data Cleaning** | Microsoft Excel, Pandas | Preprocessing, null handling, feature engineering |
| **Data Analysis** | Python, Pandas, Matplotlib, Seaborn | EDA, statistical analysis, visualisation |
| **SQL Analysis** | MySQL | Business queries, aggregations, filtering |
| **ML / Prediction** | Scikit-learn | Pattern detection, predictive analysis |
| **Dashboard** | Power BI | Interactive visual reporting |
| **Environment** | Jupyter Notebook, VS Code | Development & analysis |

---

## 🕷️ Data Acquisition — Web Scraping

Data was collected directly from **Swiggy's website** using automated scraping scripts built in Python.

### Scraping Scripts

| File | Description |
|---|---|
| `Scrapping/Swiggy Table_1.ipynb` | Scrapes restaurant names, cuisines, locations, and ratings |
| `Scrapping/Swiggy Table_2.ipynb` | Scrapes pricing, delivery time, and offer information |
| `Scrapping/Insights (1).ipynb` | Exploratory analysis and chart generation post-scraping |

### Data Points Collected

```python
# Data points scraped per restaurant listing:
{
  "restaurant_name":   "String",
  "cuisine_type":      ["North Indian", "Chinese", ...],
  "location":          "Area, Bangalore",
  "avg_cost_for_two":  Integer (INR),
  "customer_rating":   Float (0.0 – 5.0),
  "delivery_time":     Integer (minutes),
  "offers_available":  Boolean
}
```

> ⚠️ **Note:** Swiggy restaurant listings are only active during business hours, so scraping was scheduled during the **11 AM – 10 PM** window.

---

## 🧹 Data Preprocessing

After scraping, the raw data went through a rigorous cleaning pipeline:

- **Null Value Treatment** — Missing ratings and pricing filled using area-wise medians
- **Duplicate Removal** — Duplicate restaurant entries across locations identified and dropped
- **Data Type Normalization** — Delivery time (string → int), cost (₹ symbol stripped → int)
- **Feature Engineering** — Created `price_band` (Budget / Mid-range / Premium) and `is_top_rated` (rating ≥ 4.0) columns
- **Outlier Handling** — Delivery times > 90 min flagged and filtered
- **Final Dataset** → Exported as `Data/Final_Data.csv`

---

## 🗄️ SQL Analysis

The cleaned dataset was loaded into **MySQL** for structured business querying.

### Sample Business Questions Answered via SQL

```sql
-- Top 10 highest-rated restaurants in Koramangala
SELECT restaurant_name, rating, cuisine, avg_cost
FROM swiggy_data
WHERE location = 'Koramangala'
ORDER BY rating DESC
LIMIT 10;

-- Average delivery time by area
SELECT location, ROUND(AVG(delivery_time), 2) AS avg_delivery_time
FROM swiggy_data
GROUP BY location
ORDER BY avg_delivery_time ASC;

-- Most popular cuisines by restaurant count
SELECT cuisine, COUNT(*) AS restaurant_count
FROM swiggy_data
GROUP BY cuisine
ORDER BY restaurant_count DESC
LIMIT 10;

-- Price band distribution across city
SELECT
  CASE
    WHEN avg_cost <= 200 THEN 'Budget (≤₹200)'
    WHEN avg_cost <= 500 THEN 'Mid-Range (₹200–500)'
    ELSE 'Premium (>₹500)'
  END AS price_band,
  COUNT(*) AS count
FROM swiggy_data
GROUP BY price_band;

-- Areas with highest concentration of top-rated (4.0+) restaurants
SELECT location, COUNT(*) AS top_rated_count
FROM swiggy_data
WHERE rating >= 4.0
GROUP BY location
ORDER BY top_rated_count DESC;
```

---

## 💡 Key Insights

### 🏷️ Delivery Time & Customer Ratings
- Delivery time shows **limited direct correlation** with ratings overall
- But restaurants rated **4.0+** consistently deliver within **25–35 minutes**
- Delivery beyond **45 minutes** correlates with below-average customer ratings

### 🏷️ Pricing & Customer Satisfaction
- Pricing has a **marginal effect** on ratings
- **Mid-range restaurants (₹200–₹500 for two)** receive the highest order volumes
- Premium restaurants sustain ratings through quality, not pricing alone

### 🏷️ Cuisine Demand
- **North Indian, Chinese, and Biryani** dominate order volumes city-wide
- Healthy/salad-focused options are trending in tech corridors (HSR, Whitefield)
- Multi-cuisine menus outperform single-cuisine in overall rating consistency

### 🏷️ Location Intelligence
- **Koramangala, Indiranagar, and Ashok Nagar** have the highest restaurant density and customer demand
- These three areas form a central triangle — the ideal zone for a cloud kitchen
- Restaurants in these zones receive **20–30% higher order frequency** vs outer Bangalore areas

---

## 🎯 Strategic Recommendation

> **Recommendation: Establish a remote kitchen at the geographic midpoint of Koramangala – Indiranagar – Ashok Nagar.**

| Factor | Recommendation |
|---|---|
| 📍 **Location** | Central zone between Koramangala – Indiranagar – Ashok Nagar |
| 🍽️ **Cuisine** | North Indian + Chinese (high demand, proven margins) |
| 💰 **Price Point** | ₹250–₹400 for two (mid-range sweet spot) |
| ⏱️ **Delivery Target** | < 30 minutes (critical threshold for high ratings) |
| 🏆 **Differentiator** | Consistent quality + peak-hour discount offers |

**Why this location?**
- Covers 3 high-density zones from a single kitchen — maximising reach
- Shorter delivery distances lower per-order operational cost
- Balanced market presence reduces dependency on any single area
- Ideal launchpad for phased expansion into adjacent Bangalore zones

---

## 📁 Project Structure

```
swiggy_Food_Delivery/
│
├── 📂 Data/
│   └── Final_Data.csv                    # Cleaned & processed dataset
│
├── 📂 Scrapping/
│   ├── Swiggy Table_1.ipynb              # Web scraping — Part 1
│   ├── Swiggy Table_2.ipynb              # Web scraping — Part 2
│   └── Insights (1).ipynb               # EDA & visualisation notebook
│
├── 📂 New folder/
│   ├── Food Delivery (1).pdf             # Full project report
│   └── Swiggy project (Questions).sql   # SQL queries
│
├── Swiggy Dashboard.pbix                 # Power BI interactive dashboard
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install selenium pandas matplotlib seaborn beautifulsoup4 openpyxl
```

Also required:
- **Google Chrome** + matching **ChromeDriver**
- **MySQL Workbench** (for SQL analysis)
- **Power BI Desktop** — [Download here](https://powerbi.microsoft.com/desktop)

### 1. Run Scraping Notebooks

```bash
jupyter notebook
# Run in order:
# 1. Scrapping/Swiggy Table_1.ipynb
# 2. Scrapping/Swiggy Table_2.ipynb
# 3. Scrapping/Insights (1).ipynb
```

### 2. Load Data into MySQL

```sql
CREATE DATABASE swiggy_analysis;
USE swiggy_analysis;

LOAD DATA INFILE '/your/path/to/Final_Data.csv'
INTO TABLE swiggy_data
FIELDS TERMINATED BY ','
ENCLOSED BY '"'
LINES TERMINATED BY '\n'
IGNORE 1 ROWS;
```

### 3. Open Power BI Dashboard

1. Open **Power BI Desktop**
2. File → Open → `Swiggy Dashboard.pbix`
3. Update the data source path to your local `Final_Data.csv`
4. Click **Refresh** to load data

---

## 🧩 Challenges & Learnings

### 🛡️ Challenges Faced

| Challenge | Solution |
|---|---|
| Swiggy blocks automated scrapers | Randomized delays + user-agent rotation in Selenium |
| Data only available during business hours | Scheduled scraping runs during 11 AM – 10 PM windows |
| Inconsistent formats (e.g., "₹200 for two") | Regex-based parsing with Pandas for normalization |
| Missing ratings for newly listed restaurants | Imputed using area-wise median ratings |
| Power BI slowing on large dataset | Applied query folding + DAX measure optimization |

### 🎓 Key Learnings

- Real-world scraping requires patience — websites frequently change their DOM structure
- Data cleaning accounts for ~60% of any data analytics project's effort
- SQL is essential for fast, accurate slicing of large datasets before visualization
- Power BI map visuals are extremely powerful for location-based business decisions
- Data-driven location strategy consistently outperforms intuition-based decisions

---

## 🔮 Future Scope

- [ ] 🔄 **Automated pipeline** — Daily data refresh using Apache Airflow or cron jobs
- [ ] 🤖 **Demand forecasting** — LSTM/Prophet model to predict order volumes by area and hour
- [ ] 📲 **Streamlit web app** — Convert the dashboard into a publicly accessible web app
- [ ] 🗺️ **Multi-city expansion** — Scale to Mumbai, Delhi, Hyderabad, Chennai
- [ ] 💬 **Sentiment analysis** — NLP on customer reviews for deeper qualitative insights
- [ ] 📦 **Menu optimization** — ML model to recommend ideal dish count and categories per location

---

⭐ **Star this repo if you found it helpful!** ⭐

*Built with 🧡 and a lot of data — because every great restaurant deserves to be found.*

</div>

