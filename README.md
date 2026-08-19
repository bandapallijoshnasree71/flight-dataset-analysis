### 📄 Project 2: Flight Fare Intelligence & Exploratory Data Analysis

```markdown
# ✈️ Domestic Airline Pricing Intelligence: Exploratory Data Analysis (EDA)

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-Analytics-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Seaborn-Statistical_Viz-3776AB?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Matplotlib-Plotting-11557C?style=for-the-badge" />
</p>

## 📌 Executive Summary
An in-depth statistical and exploratory analysis of domestic airfare dynamics based on **26,000+ flight records**. This project evaluates how travel class, route duration, layover frequencies, departure time-blocks, and dynamic booking lead times affect consumer ticket costs.

---

## 🎯 Analytical Highlights & Business Findings
* **Price Skewness & Density:** Applied KDE (Kernel Density Estimation) and histogram distributions to uncover multimodal fare structures between economy and premium cabin tiers.
* **Lead-Time Price Elasticity:** Assessed exponential fare hikes and variance as `days_left` approaches departure.
* **Flight Duration vs. Fare:** Modeled regression trends confirming positive cost correlation with travel duration and intermediate layovers.
* **Carrier Market Share:** Mapped operational frequency across major carriers (Vistara, Air India, SpiceJet, AirAsia) to evaluate airline pricing strategies.

---

## 📈 Visual Explorations

| Chart Type | Analytical Purpose | Target Dimension |
| :--- | :--- | :--- |
| **Histplot + KDE** | Evaluates overall ticket price distribution and skewness. | `price` |
| **Boxplot** | Pinpoints price variance, quartile spreads, and outlier fare spikes. | `price` |
| **Pie Chart** | Assesses proportional flight density and carrier market share. | `airline` |
| **Regplot & Scatter** | Investigates linear pricing relationships with route duration. | `price` vs. `duration` |
| **Multivariate Pairplot**| Evaluates multi-dimensional interactions across operational metrics. | `stops`, `duration`, `days_left`, `price` |

---

## 📁 Dataset Schema

| Attribute | Type | Description |
| :--- | :--- | :--- |
| **`airline`** | Categorical | Airline operator |
| **`flight`** | String | Unique flight identifier code |
| **`source_city`** | Categorical | Origin departure city |
| **`departure_time`** | Categorical | Departure time window (Morning, Evening, Night, etc.) |
| **`stops`** | Categorical | Number of layovers (zero, one, two+) |
| **`arrival_time`** | Categorical | Arrival time window |
| **`destination_city`** | Categorical | Final destination city |
| **`class`** | Categorical | Cabin tier (Economy / Business) |
| **`duration`** | Float | Total travel time in hours |
| **`days_left`** | Integer | Booking lead time (days before flight) |
| **`price`** | Float / Int | Ticket fare |

---

## 💻 Tech Stack
* **Language:** Python 3.8+
* **Data Processing:** Pandas, NumPy
* **Visualization:** Seaborn, Matplotlib

---

## 🚀 Quickstart
```bash
# Clone the repository
git clone [https://github.com/](https://github.com/)<your-username>/flight-price-eda.git

# Install requirements
pip install pandas numpy seaborn matplotlib

# Run the notebook
jupyter notebook Flightdataset.ipynb
