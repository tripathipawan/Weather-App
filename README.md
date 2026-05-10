# 🌤️ Weather App

A real-time weather dashboard that fetches live weather data from an external API — showing current conditions and a 5-day forecast for any city searched by name or using the device's current location. Built with HTML, CSS, and JavaScript.

---

## 📌 Overview

This Weather Dashboard allows users to look up current weather conditions for any city worldwide by typing a city name and clicking Search, or by using their device's GPS via the "Use Current Location" button. The app displays temperature, wind speed, and humidity for the current moment, plus a 5-day forecast with the same data points for each upcoming day. All weather data is fetched live from an external weather API through JavaScript.

---

## ✨ Features

- **City Name Search (`.city-input`)** — A text input with placeholder `"E.g., New york, London, India"` where users type any city name to fetch its weather.
- **Search Button (`.search-btn`)** — Triggers the API call using the city name entered in the input field.
- **Use Current Location Button (`.location-btn`)** — Uses the browser's Geolocation API to detect the user's current coordinates and fetch weather for their exact location automatically — no city name needed.
- **Visual Separator (`.separator`)** — A divider between the "Search" and "Use Current Location" options, making the two input methods visually distinct.
- **Current Weather Panel (`.current-weather`)** — Displays the following for the searched or detected location:
  - City name and country code
  - Temperature in **°C**
  - Wind speed in **M/S**
  - Humidity in **%**
- **5-Day Forecast Section (`.days-forecast`)** — Shows weather cards for the next 5 days, each card displaying:
  - Date
  - Temperature in **°C**
  - Wind speed in **M/S**
  - Humidity in **%**
- **5 Forecast Cards (`.card`)** — Each of the 5 upcoming days gets its own card in a `.weather-cards` list, all dynamically populated by JavaScript from the API response.
- **Live API Data** — JavaScript (47.1% of the codebase) handles all API requests, JSON parsing, and DOM population — no data is hardcoded.
- **Responsive Design** — CSS media queries ensure the dashboard layout adapts cleanly to desktop, tablet, and mobile screen sizes.
- **No Dependencies** — Pure HTML, CSS, and JavaScript. Requires an internet connection for API and geolocation data.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Dashboard structure — search input, location button, current weather panel, 5-day forecast cards |
| CSS3 | Styling — weather card layout, dashboard grid, responsive breakpoints |
| JavaScript (ES6+) | API fetch, Geolocation API, JSON parsing, dynamic DOM population for all weather fields |
| External Weather API | Provides live current weather and 5-day forecast data |

> **Note:** JavaScript accounts for **47.1%** of the codebase, reflecting the weight of the API integration, geolocation handling, and full DOM rendering logic.

---

## 📁 Project Structure

```
Weather-App/
├── Index.html    # Main HTML — search input, location button, current weather section, 5-day forecast cards
├── Style.css     # All styling — dashboard layout, weather cards, responsive media queries
├── Script.js     # Core logic — API call, geolocation, JSON parsing, weather data DOM updates
└── README.md     # Project documentation
```

---

## 🚀 Getting Started

**1. Clone the repository**
```bash
git clone https://github.com/tripathipawan/Weather-App.git
```

**2. Navigate into the project folder**
```bash
cd Weather-App
```

**3. Add your API key**

Open `Script.js` and insert your weather API key in the appropriate variable. A free key can be obtained from [OpenWeatherMap](https://openweathermap.org/api) or the relevant API provider.

**4. Open in browser**
```
Open Index.html in any modern browser
— or use VS Code Live Server
```

> **Note:** An active internet connection is required for live API data and geolocation to work.

---

## 🧭 How to Use

**Option 1 — Search by City Name:**
1. Type a city name into the search input (e.g., `London`, `New York`, `Mumbai`).
2. Click the **Search** button.
3. Current weather and 5-day forecast load for that city.

**Option 2 — Use Current Location:**
1. Click the **"Use Current Location"** button.
2. Allow browser location access when prompted.
3. Weather for your current location loads automatically.

---

## 🌱 What I Learned

- Fetching live weather data from a REST API using JavaScript `fetch()` with query parameters (city name and coordinates)
- Using the browser's Geolocation API (`navigator.geolocation`) to get the user's current latitude and longitude
- Parsing multi-level JSON responses to extract temperature, wind speed, humidity, and forecast dates
- Dynamically building and injecting 5 forecast card elements into the DOM from API data
- Handling two distinct user input flows (manual city search vs auto-location) within one JavaScript module

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve this project:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature-name`)
3. Commit your changes (`git commit -m 'Add: your feature description'`)
4. Push to the branch (`git push origin feature/your-feature-name`)
5. Open a Pull Request

---

## 👨‍💻 Author

**Pawan Tripathi**
- GitHub: [@tripathipawan](https://github.com/tripathipawan)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
