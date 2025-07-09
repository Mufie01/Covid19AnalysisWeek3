# COVID-19 Data Analysis Project

Hi! This is Mohmed Sayeed Mufeezdeen from Crescent Institute of Sciecne and Technology. This is a Data Science exploratory project for **Week 3 (NSP Nexus Program)** analyzing the global spread and impact of COVID-19 using real-world data. The project utilizes **Python**, **Pandas**, **Matplotlib**, and **Seaborn** to generate visual insights from the dataset.

---

## Objective

The goal of this project is to perform **Exploratory Data Analysis (EDA)** on publicly available COVID-19 data to:

- Understand trends in confirmed cases, deaths, and population impacts globally.
- Visualize and compare the COVID-19 situation among various countries.
- Practice working with large datasets and Python data visualization libraries.
- Gain insights through clean, readable, and insightful visualizations.

---

## Tools & Libraries Used

- **Python 3.x**
- **Jupyter Notebook / Google Colab**
- **Libraries**:
  - `pandas` – for data manipulation
  - `numpy` – for numerical operations
  - `matplotlib` – for basic plotting
  - `seaborn` – for advanced visualizations

---

## Dataset Used

- Source: [Our World in Data (OWID)](https://ourworldindata.org/coronavirus)
- Download Link (CSV):  
  [https://covid.ourworldindata.org/data/owid-covid-data.csv](https://covid.ourworldindata.org/data/owid-covid-data.csv)

### Key Columns in the Dataset

- `date`
- `location` (country name)
- `total_cases`
- `new_cases`
- `total_deaths`
- `population`
- `continent`

---

## Project Workflow

### Step 1: Load the Dataset

- Load the OWID dataset using Pandas directly from the URL.
- Display the first few rows to get an overview.

### Step 2: Clean the Dataset

- Keep only relevant columns for analysis.
- Handle missing values (e.g., drop rows without `total_cases` or `total_deaths`).
- Convert date column to datetime format for time series plots.

### Step 3: Visual Analysis

#### a. Top 10 Countries by Total COVID-19 Cases

- Visualize total cases using a horizontal bar chart.

####  b. New Cases Trend Over Time

- Plot line graphs for new daily cases in selected countries (India, USA, Brazil).

####  c. Total Deaths vs. Total Cases (Top 10)

- Compare the number of total deaths against total cases for the most affected countries.

####  d. Global Trend of New Daily Cases

- Plot global total new daily cases over time to visualize the worldwide trend.

#### e. India-specific Case Growth

- Line graph showing India's total cases over time.

###  Step 4: Bonus Metric – Death Rate Calculation

- Calculate death rate using:
  ```python
  death_rate = (total_deaths / total_cases) × 100
