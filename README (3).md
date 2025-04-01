
# 🚖 NYC Taxi Data Analysis: Ride Trends & Fare Insights

## 🧾 Project Title
**NYC Taxi Data Analysis: Ride Trends & Fare Insights**

---

## 📌 Introduction

This project analyzes a real-world NYC taxi dataset containing trip records from March 2019. It explores ride patterns, fare structures, and tip behaviors based on location and time of day. Using Python's pandas and visualization libraries, this project extracts insights such as:

- Ride volume by hour and date
- Payment method distributions
- Average fares, tips, and ride durations
- Borough-level pickup/dropoff trends
- Top 10 highest fare rides

The goal is to showcase real-world data analysis skills while identifying business-relevant KPIs for decision-making in transportation and urban mobility.

---

## ⚙️ Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/nyc-taxi-data-analysis.git
cd nyc-taxi-data-analysis
```

2. **Set up a virtual environment (optional but recommended)**
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Open the Jupyter notebook**
```bash
jupyter notebook notebooks/analysis.ipynb
```

---

## 📈 Usage

After loading the dataset (`Taxis_Data.xlsx`), the notebook walks you through:

### 🕒 Analyzing Ride Trends by Hour & Date
```python
df['pickup_hour'] = df['pickup'].dt.hour
df['pickup_date'] = df['pickup'].dt.date

# Ride count by hour
df['pickup_hour'].value_counts().sort_index()

# Ride count by day
df['pickup_date'].value_counts().sort_index()
```

### 📊 Calculating KPIs
- Average fare per mile
- Tip percentage
- Total revenue (fare + tip + tolls)
```python
df['fare_per_mile'] = df['fare'] / df['distance']
df['tip_pct'] = df['tip'] / df['fare'] * 100
df['revenue'] = df['fare'] + df['tip'] + df['tolls']
```

### 🔍 Top 10 Highest Fare Rides
```python
df.nlargest(10, "fare")
```

### 📊 Plotting Ride Trends
```python
import matplotlib.pyplot as plt

df['pickup_hour'].value_counts().sort_index().plot(kind='bar', figsize=(10,5))
plt.title("Total Rides by Hour of Day")
plt.xlabel("Hour of Day")
plt.ylabel("Number of Rides")
plt.grid(True)
plt.show()
```

---

## 🤝 Contributing

Contributions are welcome! Here’s how you can help:

### 📥 Pull Requests
- Fork the repository
- Create a new branch (`git checkout -b feature/your-feature`)
- Commit your changes (`git commit -m 'Add some feature'`)
- Push to the branch (`git push origin feature/your-feature`)
- Open a pull request

### 🐞 Reporting Issues
If you find a bug or would like to request a new feature, please open an issue with:
- A clear title
- Steps to reproduce
- Screenshots if applicable

### 💡 Suggestions
Feel free to suggest improvements to analysis, visuals, or project structure. Let’s collaborate and make this project even better!

---

## 📃 License

This project is open source under the [MIT License](LICENSE).

---

## 🙋 Contact

Made by [Your Name] – [LinkedIn](https://linkedin.com/in/your-profile) | [GitHub](https://github.com/yourusername)

Got feedback or ideas? Let’s connect!
