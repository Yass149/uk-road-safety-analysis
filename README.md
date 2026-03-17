# UK Road Safety Analysis (2024)

## Project Overview
This project provides a comprehensive analysis of the **UK Road Casualty dataset (2024)**. The primary focus is to demonstrate a robust data science workflow, including advanced data cleaning, handling of domain-specific missing values, and exploratory data analysis (EDA) to uncover safety trends.

### Key Objectives
* **Data Wrangling:** Process a large-scale dataset (>128k records) using Python and Pandas.
* **Handling Metadata:** Identify and manage non-standard missing value placeholders (e.g., -1 and 9).
* **Insight Generation:** Analyze the distribution and severity of road casualties to identify high-risk categories.

---

## Tech Stack
* **Language:** Python 3.x
* **Libraries:** * `Pandas`: Data manipulation and structural analysis.
    * `Matplotlib` & `Seaborn`: Statistical data visualization.
* **Environment:** Jupyter Notebook.

---

## Dataset Description
The analysis utilizes the official UK Road Casualty data. Each record represents a unique casualty incident with 23 distinct features, including:
* **Demographics:** Age, sex, and casualty class.
* **Severity:** Categorized as Fatal, Serious, or Slight.
* **Context:** Collision year, vehicle reference, and geographical IMD (Index of Multiple Deprivation) deciles.

---

## Project Pipeline

### 1. Data Loading & Inspection
Initial audit of the `casualties.csv` file to understand the schema, memory usage (~22.5 MB), and identify data types for 128,272 entries.

### 2. Data Cleaning & Pre-processing
* **Placeholder Management:** Replaced domain-specific placeholders (like `-1` in `age_of_casualty`) with `pd.NA` to ensure statistical accuracy.
* **Type Conversion:** Standardized numerical columns for optimized mean and distribution calculations.
* **Validation:** Verified the integrity of the data post-cleaning (e.g., calculating a realistic average casualty age of 38.31 years).

### 3. Exploratory Data Analysis (EDA)
Created visual representations of casualty severity to understand the impact of road incidents. 
* **Key Insight:** The vast majority of casualties are classified as "Slight," but the distribution of "Serious" and "Fatal" incidents provides critical focus areas for road safety policy.

---

## How to Run
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/uk-road-safety-analysis.git](https://github.com/your-username/uk-road-safety-analysis.git)
