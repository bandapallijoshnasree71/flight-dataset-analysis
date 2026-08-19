# ✈️ Flight Price Dynamics: Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project performs an Exploratory Data Analysis (EDA) on domestic airline ticket pricing across 26,000+ flight records. It investigates the impact of booking lead time (`days_left`), flight duration, departure timing, and carrier market share on consumer ticket prices.

---

## 🎯 Key Objectives & Analytical Dimensions
* **Price Distribution:** Evaluated price spread across economy/business classes and identified right-skewed pricing distributions.
* **Duration vs. Price:** Measured how stopovers and travel duration affect overall pricing using linear regression models.
* **Market Share & Airlines:** Analyzed ticket volume distribution across domestic carriers (SpiceJet, AirAsia, Vistara, Air India).
* **Booking Lead Time:** Examined price appreciation as flight departure dates approach.

---

## 📈 Visualizations & Statistical Insights

* **Univariate Price Distribution (Histplot + KDE):** Analyzed the multimodal nature of ticket prices and visualizes fare distributions.
* **Outlier Detection (Boxplot):** Identified premium pricing tiers and outlier fare spikes across standard bookings.
* **Airline Market Distribution (Pie Chart):** Broke down the proportional flight frequency per airline carrier.
* **Duration vs. Fare Regression (Scatter & Regplot):** Evaluated correlation trends between flight hours and final fare prices.

---

## 📁 Dataset Attributes

| Field Name | Type | Description |
| :--- | :--- | :--- |
| `airline` | Categorical | Airline carrier operating the flight |
| `flight` | String | Unique flight code/number |
| `source_city` | Categorical | Departure origin city |
| `departure_time` | Categorical | Departure time-block (Morning, Evening, Night, etc.) |
| `stops` | Categorical | Number of transit stops (zero, one, two+) |
| `arrival_time` | Categorical | Arrival time-block |
| `destination_city` | Categorical | Arrival destination city |
| `class` | Categorical | Travel cabin class (Economy / Business) |
| `duration` | Float | Total travel time in hours |
| `days_left` | Integer | Days remaining between booking date and flight departure |
| `price` | Float / Int | Final ticket fare in target currency |

---

## 💻 Tech Stack
* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Visualization:** Seaborn, Matplotlib
* **Environment:** Google Colab / Jupyter Notebook

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/<your-repo-name>.git
