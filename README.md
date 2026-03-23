# Data Analysis: Socioeconomic Indicators in Chicago (2008–2012)


This project analyzes the relationship between various public health significance indicators and the overall "Hardship Index" across 77 community areas in Chicago. Using a combination of **SQL** and **Python**, we explore how economic factors like per-capita income correlate with social challenges.

## 📊 Dataset Overview
The dataset was sourced from the Chicago City Portal and contains:
* **6 Socioeconomic Indicators**: Housing crowding, poverty levels, unemployment, education levels, and demographic dependency.
* **Hardship Index**: A score from 1 to 100 (higher = more hardship) that incorporates all six indicators.
* **Timeframe**: 2008 – 2012.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Database:** SQLite
* **Libraries:** * `pandas` (Data manipulation)
    * `ipython-sql` (Magic SQL functions)
    * `matplotlib` & `seaborn` (Data visualization)

## 🚀 Getting Started

### 1. Prerequisites
Ensure you have the required libraries installed:
```bash
pip install pandas ipython-sql matplotlib seaborn
```

### 2. Database Setup
The notebook automatically converts the raw `chicago-socioeconomic_indicators_2008_2012.csv` into a SQLite database (`chicago_socioeconomic.db`) to allow for SQL-based exploration.

### 3. Running the Analysis
1. Open the Jupyter Notebook: `chicago-socioeconomic-sql-analysis.ipynb`.
2. Execute the cells in order to:
    * Load and clean the data.
    * Establish the SQL connection via `%load_ext sql`.
    * Perform exploratory queries.
    * Generate the correlation scatter plots.

## 📈 Key Findings
* **Max Hardship:** The community area of **Riverdale** recorded the highest hardship index of **98**.
* **Wealth Clusters:** Only 4 areas (Near North Side, Lincoln Park, Loop, and Lake View) maintain a per-capita income above **$60,000**.
* **Correlation:** We found a **strong negative correlation (~ -0.85)** between per-capita income and the hardship index, visually confirmed via regression analysis.


## 📝 License
This project is open-source. Data is provided by the City of Chicago.

