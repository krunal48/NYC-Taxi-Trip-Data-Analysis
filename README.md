# 🛺 NYC Taxi Trip Data Analysis

This repository contains an exploratory data analysis of NYC taxi rides from March 2019. The goal is to derive key insights from taxi ride behavior, payment methods, tip trends, and borough-level movement using Python and its powerful data manipulation libraries.

---

## 📁 Dataset Description

- **File**: `Taxis_Data.xlsx`
- **Sheet**: `Taxis`
- **Records**: 6,433 taxi rides
- **Fields**:
  - `pickup`, `dropoff`: datetime of pickup and dropoff
  - `passengers`: number of passengers
  - `distance`: distance of the trip (miles)
  - `fare`: base fare for the trip
  - `tip`: tip amount given
  - `tolls`: any tolls paid during the trip
  - `total`: total amount paid (fare + tip + tolls)
  - `color`: cab color (e.g. yellow, green)
  - `payment`: payment method (e.g. credit card, cash)
  - `pickup_zone`, `dropoff_zone`: neighborhood zones
  - `pickup_borough`, `dropoff_borough`: NYC boroughs

---

## 🧪 Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib & Seaborn
- Jupyter Notebook / Google Colab

---

## 📊 Key Performance Indicators (KPIs)

1. **Average Fare per Mile**
2. **Total Revenue (Fare + Tip + Tolls)**
3. **Average Tip Percentage**
4. **Most Common Pickup & Dropoff Zones**
5. **Rides by Payment Type**
6. **Average Ride Duration and Distance**
7. **Hourly Pickup Trend**
8. **Passenger Count Distribution**
9. **Rides per Borough**
10. **Daily Ride Count**


##🔑 **Insights**

Credit cards were the most preferred payment method.

Tips averaged between 15–20% of the fare.

Most rides were short (~1–3 miles) with 1–2 passengers.

Manhattan dominated both pickup and dropoff activity.

Ride volume peaked during rush hours and weekends.

---

## ⚙️ Installation

1. **Clone the repository**
```bash
git clone https://github.com/krunal48/NYC-Taxi-Trip-Data-Analysis
cd NYC-Taxi-Trip-Data-Analysis
```

2. **Set up a virtual environment (optional but recommended)**
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install pandas
pip install openpyxl
pip install seaborn
pip install matplotlib.pyplot
```

4. **Open the Jupyter notebook**
```bash
jupyter notebook notebooks/Taxi_Trip_Data_Analysis.ipynb
```

---


### 💡 Suggestions
Feel free to suggest improvements to analysis, visuals, or project structure. Let’s collaborate and make this project even better!

---

## 🙋 Contact

Made by Krunal Soni – [LinkedIn](https://www.linkedin.com/in/krunal-v-soni/) | [GitHub](https://github.com/krunal48)

Got feedback or ideas? Let’s connect!
