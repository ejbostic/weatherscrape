# 🌍 NYC Historical Weather Analysis & Visualization

This project analyzes and visualizes over 200 years of historical weather data for New York City using the [Meteostat](https://dev.meteostat.net/) API. It includes temperature and precipitation trends, comparisons over time, and seasonal/monthly breakdowns.

---

## 📦 Features

- Daily temperature data (min, max, average) from **1800 to present**
- **5-year rolling average** of daily temperatures to observe long-term climate trends
- Comparison of **monthly average precipitation** (historical vs. recent 12 months)
- Monthly breakdown of **average**, **minimum**, and **maximum** temperatures
- Visualization of **January vs July** average temperature trends over time
- Clean, informative Matplotlib visualizations

---

## 📊 Visualizations Included

1. **Long-Term Daily Temperature Trend (°F)**  
   Shows average daily temperature and 5-year rolling trendline from 1800 to today.

2. **Change in Temperature Over 200+ Years**  
   Highlights the difference between earliest and latest 5-year rolling averages.

3. **Average Monthly Rainfall (inches)**  
   Historical average vs. last 12 months.

4. **Average Monthly Midpoint Temperatures (°F)**  
   Comparison of historical average vs. last 12 months.

5. **January vs July Temperature Trends Over Time (°F)**  
   Long-term plot showing how temperatures in the coldest and hottest months have shifted.

6. **Average Monthly Min and Max Temperatures (°F)**  
   Historical vs. recent comparison for both minimum and maximum values.

---

## 🧪 Dependencies

Install the required Python packages using:

```bash
pip install matplotlib pandas meteostat
```

---

## 📍 Cities Defined (for easy expansion)

Though the main visualizations focus on NYC, other cities are predefined and can be swapped easily:

```python
nyc = Point(40.7128, -74.0060)
london = Point(51.5074, -0.1278)
tokyo = Point(35.6762, 139.6503)
sydney = Point(-33.8688, 151.2093)
paris = Point(48.8566, 2.3522)
berlin = Point(52.52, 13.4050)
cape_town = Point(-33.9249, 18.4241)
mumbai = Point(19.0760, 72.8777)
rio = Point(-22.9068, -43.1729)
toronto = Point(43.65107, -79.347015)
moscow = Point(55.7558, 37.6173)
```

To analyze a different city, simply replace `moscow` with any of the above.

---

## 📅 Date Range

- **Start**: January 1, 1800  
- **End**: Current date (automatically updated)

---

## 🧠 How It Works

- Fetches historical daily data using the `Meteostat` API
- Converts temperature and precipitation to **Fahrenheit** and **inches**
- Aggregates and smooths data using **rolling averages** and **monthly groupings**
- Plots results using `matplotlib`

---

## 📈 Sample Output

- Clear, color-coded bar and line charts
- Comparative stats for long-term vs. recent year
- Trends visualized for easier interpretation of climate change impact

---

## 🔄 Customization Tips

- Change city by modifying the `Point()` instance used.
- Adjust the rolling window by modifying `window=365*5` for different smoothing levels.
- Plot different variables by tweaking the DataFrame columns and groupings.

---

## 📍 Note

Ensure you have a stable internet connection when running this script, as the Meteostat API fetches data in real-time.

---

## 📜 License

This project is open-source and available for modification or extension.

