# FIFA World Cup — Data Scraping & 2026 Prediction

This project aims to **extract historical FIFA World Cup data** using Web Scraping from Wikipedia, build a **clean dataset of past match results**, and then use that information to **predict possible outcomes for the 2026 World Cup**.

This repository includes:
- Scraping code (`webscraping_data.ipynb`)
- Machine learning prediction code (`prediction_2026_worldcup.ipynb`)
- Datasets generated through scraping (CSV)

---

## 1. Project Objective

1. **Collect historical data** from all World Cups from 1930 to 2018.  
2. **Clean, structure, and store** that data into CSV files.  
3. **Train machine learning models** to analyze result patterns.  
4. **Predict outcomes for the 2026 World Cup** using historical features.

---

## 2. Repository Contents

/
├── prediction_2026_worldcup.ipynb # Predictive model for the 2026 World Cup
├── clean_csv_files-format_fixtures.ipynb # Cleaning and formatting of CSV files
├── data/
│ ├── clean_fifa_worldcup_historical_data.csv
│ ├── fifa_worldcup_fixture_2026.csv
│ ├── fifa_worldcup_historical_data.csv
│ ├── fifa_worldcup_missing_data.csv
│ ├── grupos_2026.json
│ └── format_fixture_data.csv
├── scrapping/
│ ├── Web_Scrapping_bs4.ipynb
│ └── Web_Scrapping_selenium.ipynb
└── README.md

---

## 3. Web Scraping

The `scrapping` folder contains:

### **`Web_Scrapping_bs4.ipynb`**

- Extracts match results for each World Cup edition  
- Skips the years not played (1942 and 1946)  
- Provides a step-by-step guide using `requests`, `BeautifulSoup`, and `pandas`  
- Generates clean datasets for later analysis  

**Technologies used:**
- `requests`
- `BeautifulSoup4`
- `pandas`
- `lxml`

### **`Web_Scrapping_selenium.ipynb`**

- Extracts match results for all World Cups, including missing years  
- Skips editions not played (1942 and 1946)  
- Automates navigation through Wikipedia using Selenium  
- Selects elements via XPath  
- Stores data in a ready-to-analyze CSV file  

**Technologies used:**
- `selenium`
- `pandas`
- `time`
- `chromedriver` / `Chrome WebDriver`

---

## 4. Dataset Cleaning and Formatting

In the notebook **`clean_csv_files-format_fixtures.ipynb`**:

- Scraped datasets are cleaned and normalized  
- `df_fixture` is formatted to create a preliminary version of the 2026 World Cup  
- This workflow allows working with the dataset even though the remaining 18 qualifying teams are still unknown  
- This code create the file 'grupos_2026.json' for the tables with the groups in the WorldCup 2026
---

## 5. 2026 World Cup Prediction

In **`prediction_2026_worldcup.ipynb`**:

- Historical data generated during scraping is loaded  
- Features such as goals, goal differences, historical performance, etc. are created  
- A machine learning model is trained (RandomForest, XGBoost, or others)  
- Predictions for the 2026 matches are generated  

---

## Author

**Pool Jinez**

---

## Credits

These exercises were carried out following the guidance of YouTuber **Frank Andrade**  
Channel: https://www.youtube.com/@thepycoachES

These are practice projects created to keep a record of the code used and support self-taught learning while improving my skills in **Data Science**.
