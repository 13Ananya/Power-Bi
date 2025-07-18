# 🌦️ Real-Time Weather Forecasting Dashboard using Power BI & WeatherAPI.com

This project presents a dynamic **real-time weather forecasting dashboard** built using **Power BI**, powered by data fetched directly from **WeatherAPI.com**. It visualizes live weather metrics across six key locations in India: **Roha**, **Mumbai**, **Pune**, **Ratnagiri**, **Udupi**, and **Mangalore**.

---

## 🎯 Why WeatherAPI?

[WeatherAPI.com](https://www.weatherapi.com/) is a simple yet powerful weather data provider that delivers:

- ✅ Real-time weather data
- ✅ Historical and forecast reports
- ✅ Air Quality Index (AQI) information

It offers data in **JSON format**, which makes it easy to extract and transform directly into Power BI.

---

## 🔧 Steps I Followed

### 🔑 Step 1: Get Your WeatherAPI Key

1. I signed up at [WeatherAPI.com](https://www.weatherapi.com/).
2. Copied my unique **API key** from the dashboard.
3. This API key is required to authenticate requests.

---

### 🌐 Step 2: Build the API URL

I constructed the API endpoint using the following format:
https://api.weatherapi.com/v1/current.json?key=YOUR_API_KEY&q=CITY_NAME


I repeated this for each of the six cities I focused on.

---

### 🧠 Step 3: Connect Power BI to WeatherAPI

1. Opened **Power BI Desktop**
2. Chose **Get Data → Web**
3. Pasted the WeatherAPI URL
4. Clicked **OK** to connect

---

### 🧹 Step 4: Transform the Data

Once Power BI loaded the JSON:

- I expanded the `current` record
- Further expanded `condition` and `air_quality` fields
- Renamed the columns for clarity and ease of use
- Clicked **Close & Apply** to load data into Power BI

---

### 📊 Step 5: Build the Dashboard

To bring the data to life, I:

- Used **cards** to display current temperature, humidity, cloud, and pressure
- Created **gauges** for wind speed and visibility
- Designed **charts** to show variations in key weather metrics
- Added **filters/slicers** to switch between cities easily

---

### 🎨 Step 6: Styling & Interactivity

- Inserted **weather icons** to represent current conditions
- Plotted **map visuals** to show geographic distribution
- Allowed users to dynamically select a city and view its weather instantly

---

### ⚡ Step 7: Adding AQI Indicators with Reusable Measures

WeatherAPI provides air quality data inside the `current.air_quality` object.

I:

- Extracted values like `pm2_5`, `pm10`, and `us-epa-index`
- Created **DAX measures** to calculate and visualize AQI
- Displayed AQI with **color indicators** to highlight pollution levels

---

## 🌍 Real-World Applications

This dashboard can be used in various real-life scenarios:

- **Disaster Management:** Track weather changes for emergency planning
- **Logistics & Supply Chain:** Adjust transport routes based on wind and visibility
- **Tourism:** Help travelers plan trips by checking real-time conditions
- **Agriculture:** Farmers can monitor temperature and humidity for crop planning
- **Health Monitoring:** Visualize AQI to issue warnings for respiratory risks


---

## ✅ Prerequisites

- Power BI Desktop installed
- Valid API key from [WeatherAPI.com](https://www.weatherapi.com/)
- Internet connection to refresh data

---

## 📈 Future Enhancements

- Add hourly & forecast data
- Incorporate weather alerts
- Schedule auto-refresh for continuous real-time insights

---

## 🙌 Thank You!

If you found this useful or want to collaborate on similar data visualization projects, feel free to connect or fork the repo!

