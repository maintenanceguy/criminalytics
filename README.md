# 🔎 Criminalytics
### Temporal & Spatial Crime Analysis of Los Angeles Crime Reports

<p align="center">
  <strong>Turning raw crime data into meaningful patterns, trends, and insights.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white">
  <img src="https://img.shields.io/badge/NumPy-Statistics-013243?style=for-the-badge&logo=numpy&logoColor=white">
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white">
</p>

---

## 📌 Overview

**Criminalytics** is a Python-based crime data analysis and visualization project focused on discovering **temporal and spatial patterns in reported crime across Los Angeles**.

The project transforms a large collection of crime records into meaningful insights through:

- Data cleaning
- Feature engineering
- Exploratory Data Analysis
- Statistical analysis
- Temporal analysis
- Spatial analysis
- Data visualization
- Crime anomaly detection

Instead of simply asking **"How many crimes occurred?"**, Criminalytics explores:

> **When does crime happen? Where does it happen? What types of crime are most common? And what unusual patterns can be found in the data?**

---

## 🎯 Project Objectives

The main objectives of Criminalytics are to:

- 📊 Analyze the most frequently reported crime types
- 📍 Identify areas with high concentrations of crime
- 🕐 Discover temporal crime patterns
- 📅 Analyze crime activity by day of the week
- 🌅 Compare crime across different times of day
- 🔫 Analyze reported weapon usage
- 👥 Explore victim demographic patterns
- 🔗 Examine relationships between crime types and time
- ⚠️ Detect unusual spikes in daily crime activity
- 📈 Identify statistically significant high-crime areas
- 🧠 Convert raw crime records into understandable insights

---

## 📂 Dataset

The project analyzes a large Los Angeles crime dataset containing **134,198 crime records**.

The dataset contains information related to:

- 📅 Date and time of incidents
- 📍 Crime locations and areas
- 🚨 Crime types
- 🔫 Weapons
- 👤 Victim information
- 🏙️ Geographic distribution
- 📈 Daily incident activity

The size and variety of the dataset allow Criminalytics to perform both **temporal** and **spatial** analysis.

---

# 🔬 Methodology

The project follows a structured data-analysis pipeline:

```text
Raw Crime Dataset
       │
       ▼
Data Cleaning
       │
       ▼
Feature Engineering
       │
       ▼
Exploratory Data Analysis
       │
       ├───────────────┐
       ▼               ▼
Temporal Analysis   Spatial Analysis
       │               │
       └───────┬───────┘
               ▼
       Statistical Analysis
               │
        ┌──────┴──────┐
        ▼             ▼
    Z-Scores     Crime Spike Detection
        │             │
        └──────┬──────┘
               ▼
        Data Visualization
               │
               ▼
        Crime Insights
```

---

## 🧹 Data Cleaning

Before analysis, the raw dataset is processed to improve consistency and usability.

The preprocessing stage includes:

- Handling missing values
- Cleaning categorical variables
- Converting date and time fields
- Preparing numerical variables
- Handling unknown weapon information
- Preparing the dataset for statistical analysis
- Removing or addressing unusable records where appropriate

---

## ⚙️ Feature Engineering

New analytical features are extracted from the original crime records.

### Temporal Features

The project extracts:

- Hour
- Day
- Day of the week
- Month
- Year
- Time of day

Crime incidents are categorized into four major periods:

| Period | Description |
|---|---|
| 🌅 Morning | Early-day activity |
| ☀️ Afternoon | Midday activity |
| 🌆 Evening | Evening activity |
| 🌙 Night | Night-time activity |

This makes it possible to compare crime patterns across different periods of the day.

---

# 📊 Exploratory Data Analysis

Criminalytics explores crime from multiple perspectives.

### 🚨 Crime Type Analysis

Identifies the most frequently reported crimes and compares their contribution to the overall dataset.

### 📍 Area Analysis

Examines how crime incidents are distributed across different areas of Los Angeles.

### 🕐 Time Analysis

Analyzes crime according to:

- Hour of day
- Time period
- Day of week
- Month
- Year

### 🔫 Weapon Analysis

Investigates weapons associated with reported incidents and identifies the most frequently recorded categories.

### 👥 Victim Analysis

Explores available victim demographic information and its relationship with different crime categories.

---

# 🔬 Statistical Analysis

Criminalytics goes beyond simple frequency counts by applying statistical techniques.

## 📈 Z-Score Analysis

Z-scores are used to identify areas whose crime counts are significantly different from the overall distribution.

This provides a statistical approach for identifying areas with unusually high crime volumes rather than relying only on raw totals.

The analysis highlights areas such as:

- **Central**
- **Southwest**
- **Pacific**

as particularly notable based on the project's statistical threshold.

---

## ⚠️ Crime Spike Detection

The project analyzes daily crime activity to detect unusual increases.

A **two-standard-deviation threshold** is used to identify days where reported crime activity is substantially higher than the normal daily level.

The analysis identified:

> **103 unusual crime-spike days**

This provides another way to investigate abnormal crime activity beyond overall averages.

---

# 🏆 Key Findings

## 🚨 Most Common Crime Types

The analysis identified the following among the most frequently reported crime categories:

| Rank | Crime Type | Incidents |
|---:|---|---:|
| 🥇 | Vehicle - Stolen | 21,823 |
| 🥈 | Burglary from Vehicle | 9,737 |
| 🥉 | Shoplifting / Petty Theft | 9,354 |
| 4️⃣ | Theft Plain / Petty | 9,246 |
| 5️⃣ | Theft of Identity | 8,288 |

These results show that property-related crimes make up a significant portion of the analyzed crime reports.

---

## 📍 Areas With the Highest Crime Counts

The areas with the highest number of recorded incidents include:

| Rank | Area | Incidents |
|---:|---|---:|
| 🥇 | Central | 10,564 |
| 🥈 | Southwest | 8,645 |
| 🥉 | Pacific | 8,538 |
| 4️⃣ | N Hollywood | 7,704 |
| 5️⃣ | 77th Street | 7,066 |

The results demonstrate that crime activity varies considerably between different areas of Los Angeles.

---

## 🕐 Crime by Time of Day

The overall distribution of reported incidents was:

| Time Period | Percentage |
|---|---:|
| ☀️ Afternoon | 27.23% |
| 🌙 Night | 26.02% |
| 🌆 Evening | 23.80% |
| 🌅 Morning | 22.95% |

This relatively balanced distribution demonstrates the importance of analyzing crime across the entire day rather than focusing on a single period.

---

# 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 **Python** | Core programming language |
| 🐼 **Pandas** | Data manipulation and analysis |
| 🔢 **NumPy** | Numerical and statistical calculations |
| 📊 **Matplotlib** | Data visualization |
| 📓 **Jupyter Notebook** | Interactive analysis |

---

# 📁 Project Structure

```text
criminalytics/
│
├── 📁 Data/
│   └── Crime_Data.csv
│
├── 📁 figures/
│   ├── fig1_time_of_day.png
│   ├── fig2_time_proportion.png
│   ├── fig3_top_crime_types.png
│   ├── fig4_top_areas.png
│   ├── fig5_area_by_time.png
│   ├── fig6_top_weapons.png
│   ├── fig7_time_vs_crime_type.png
│   ├── fig8_day_of_week.png
│   └── fig9_daily_outliers.png
│
├── 📓 Crime_analysis.ipynb
├── 📄 Final_Project_Report.pdf
└── 📖 README.md
```

---

# 📚 Project Resources

Everything required to understand and reproduce the project is included in this repository.

| Resource | Description |
|---|---|
| 📓 [Crime Analysis Notebook](Crime_analysis.ipynb) | Complete Python analysis, calculations, and visualizations |
| 📄 [Final Project Report](Final_Project_Report.pdf) | Detailed documentation of the methodology, analysis, findings, and conclusions |
| 📁 [Crime Dataset](Data/) | Dataset used for the analysis |
| 📊 [Visualization Files](figures/) | Generated charts and analytical figures |

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/maintenanceguy/criminalytics.git
```

Navigate into the project directory:

```bash
cd criminalytics
```

## 2. Install Dependencies

```bash
pip install pandas numpy matplotlib jupyter
```

## 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Crime_analysis.ipynb
```

Run the notebook cells sequentially to reproduce the analysis.

---

# 💻 Requirements

Before running Criminalytics, make sure you have:

- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib

Check your Python installation:

```bash
python --version
```

---

# 💡 Why Criminalytics?

Crime datasets can contain thousands of individual records, but raw records alone do not provide meaningful understanding.

Criminalytics transforms those records into:

```text
Raw Data
    ↓
Clean Data
    ↓
Organized Information
    ↓
Statistical Analysis
    ↓
Visualizations
    ↓
Meaningful Insights
```

The project demonstrates how Python and data-science techniques can be applied to a real-world dataset to uncover patterns that are difficult to identify from raw data alone.

The goal is not simply to determine:

> **"How many crimes occurred?"**

but to explore:

> **"When, where, and what kinds of crimes are occurring, and what patterns can we discover from the data?"**

---

# ⚠️ Limitations

The results of this project should be interpreted within the limitations of the dataset.

- The dataset represents **reported crime incidents**, not necessarily every crime that occurred.
- Crime reporting can be influenced by reporting behavior and law-enforcement practices.
- Crime counts alone do not necessarily represent the actual risk level of an area.
- Statistical relationships do not automatically imply causation.
- The analysis is intended primarily for **educational and analytical purposes**.

---

# 🔮 Future Improvements

Criminalytics can be expanded into a more advanced crime-analysis platform.

Potential improvements include:

- 🗺️ Interactive crime maps
- 📊 Interactive dashboards
- 🤖 Machine-learning-based crime prediction
- 📍 Geographic hotspot detection
- 📈 Time-series forecasting
- ⚠️ Automated anomaly detection
- 🔎 Advanced correlation analysis
- 🌐 Web-based crime analytics dashboard
- 🔄 Automated dataset updates
- 🧠 Crime classification models

---

# 🎓 Academic Purpose

This project demonstrates practical application of:

- Python programming
- Data preprocessing
- Data cleaning
- Feature engineering
- Exploratory Data Analysis
- Statistical analysis
- Data visualization
- Data interpretation
- Real-world dataset analysis

It combines programming fundamentals with practical data-analysis techniques to investigate a real-world problem.

---

# 👨‍💻 Author

### maintenanceguy

**Criminalytics — Temporal & Spatial Crime Analysis of Los Angeles Crime Reports**

Built using:

**Python • Pandas • NumPy • Matplotlib • Jupyter Notebook**

---

# ⭐ Support

If you found **Criminalytics** interesting or useful, consider giving the repository a ⭐.

It helps support the project and encourages further development.

---

<p align="center">

### 🔎 Criminalytics

<strong>Turning crime data into meaningful insights.</strong>

<br><br>

🐍 Built with Python &nbsp;•&nbsp; 📊 Driven by Data &nbsp;•&nbsp; 🔬 Powered by Analysis

</p>
