# Mini-Project-On-API
A Python-based mini project that fetches live COVID-19 data using the disease.sh API and saves it to a CSV file for further analysis using pandas. Great for learning API integration, data cleaning, and real-world data handling as a data analyst.
# 🦠 COVID-19 Live Data Tracker using Public API

This project is a **real-time COVID-19 data tracker** built using Python. It uses the public API provided by [disease.sh](https://disease.sh/) to fetch live COVID-19 data for all countries and saves it in a structured CSV format — perfect for further analysis or dashboarding.

---

## 📌 Features

- ✅ Fetches real-time COVID-19 data by country
- ✅ Uses a public API with no authentication needed
- ✅ Extracts key metrics: total cases, deaths, recovered, active, critical, and today’s cases
- ✅ Converts JSON response into a clean `pandas` DataFrame
- ✅ Saves data to `covid19_data.csv` for use in Excel, Power BI, Tableau, etc.

---

## 🌐 API Used

- **Source:** [disease.sh - Open Disease Data API](https://disease.sh/)
- **Endpoint:** `https://disease.sh/v3/covid-19/countries`

---

## 🛠️ Tech Stack

- Python
- requests
- pandas

---

## 🧠 How It Works

1. Sends a GET request to the API endpoint  
2. Parses the JSON response  
3. Normalizes the data and selects key columns  
4. Prints the first 10 rows  
5. Saves the result to `covid19_data.csv`

---

## 📸 Sample Output

| Country        | Cases     | Deaths | Recovered | Active | Critical | TodayCases | TodayDeaths |
|----------------|-----------|--------|-----------|--------|----------|------------|-------------|
| India          | 44900000  | 531000 | 44300000  | 1000   | 10       | 50         | 1           |
| USA            | 102000000 | 1110000| 100000000 | 900000 | 5000     | 4000       | 20          |

✅ Console output confirms that the data was saved to `covid19_data.csv`.

---

## ▶️ How to Run

```bash
pip install requests pandas
python covid_tracker.py
