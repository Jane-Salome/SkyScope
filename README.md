# SkyScope 🌤️

**Live Demo** → [Click here to view the app](https://genuine-cannoli-c1589c.netlify.app/)

A real-time weather forecast web application that provides live weather updates and 5-day forecasts for any city in the world, with automatic location detection using GPS coordinates.

---

## Features

- **Current Weather** — Live temperature, humidity, wind speed, and weather conditions for any city
- **5-Day Forecast** — Detailed weather predictions for the next 5 days
- **GPS Location Detection** — Automatically fetches weather based on the user's current coordinates
- **City Search** — Search weather for any city worldwide
- **Real-time Data** — Powered by the OpenWeatherMap API for accurate, up-to-date information

---

## Tech Stack

| Layer | Tools |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Node.js, Express.js |
| API | OpenWeatherMap API |
| Deployment | Netlify (Frontend) |
| Other | CORS, dotenv |

---

## Project Structure

```
├── now.html              # Main frontend interface
├── index.js              # Express backend server
├── .env                  # Environment variables (API key)
└── package.json          # Node dependencies
```

---

## How It Works

1. **City Search** — User enters a city name → backend calls OpenWeatherMap `/weather` endpoint → returns live data
2. **GPS Detection** — App fetches user's lat/lon coordinates → backend calls `/weather` with coordinates → returns local weather
3. **Forecast** — Calls OpenWeatherMap `/forecast` endpoint to retrieve 5-day predictions
4. **Display** — Frontend renders weather data with icons, temperature, humidity, and wind details

---

## Getting Started

### Prerequisites
- Node.js 18+
- OpenWeatherMap API key (free at [openweathermap.org](https://openweathermap.org/api))

### Installation

```bash
# Clone the repository
git clone https://github.com/Jane-Salome/SkyScope.git
cd SkyScope

# Install dependencies
npm install

# Create .env file and add your API key
echo "OPENWEATHER_API_KEY=your_api_key_here" > .env

# Start the server
node index.js
```

Then open `now.html` in your browser.

---

## Author

**Jane Salome D**  
B.Tech Information Technology — Sri Sairam Engineering College  
[LinkedIn](https://www.linkedin.com/in/jane-salome-d-a47a91295) | [GitHub](https://github.com/Jane-Salome)
