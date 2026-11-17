# WeatherPulse

WeatherPulse is a sleek, real-time weather application for cities worldwide. It provides hourly updates, a 7-day forecast, UV index, wind details, sunrise/sunset timing, and a responsive mobile-friendly interface built with React and Capacitor.

## Features

- Search weather by city name
- Real-time weather data for current conditions
- Hourly forecast for the next 24 hours
- 7-day forecast overview
- UV index and wind information
- Sunrise and sunset times
- Temperature unit toggle (°C / °F)
- Light and dark theme support
- Mobile-ready design with PWA and Capacitor support
- Geolocation-based weather lookup

## Tech Stack

- React 19
- Vite
- JavaScript
- CSS / Responsive UI design
- Open-Meteo API for weather and geocoding
- Capacitor for Android app packaging

## Project Structure

```bash
Weather-App/
├── android/                 # Capacitor Android project
├── public/                  # Static public assets
├── src/
│   ├── App.css              # App styling
│   ├── App.jsx              # Main weather dashboard UI
│   ├── SkyBackground.jsx    # Animated weather background
│   ├── index.css            # Global styles
│   ├── main.jsx             # React entry point
│   ├── weatherUtils.js      # Weather and geocoding helper functions
│   └── ...
├── .gitignore
├── index.html
├── package.json
├── README.md
├── vite.config.js
└── ...
```

## Prerequisites

Before running the project, make sure you have the following installed:

- Node.js (v18 or newer recommended)
- npm
- Android Studio (optional, only for Android build)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/Yugandhar2024/Weather-App.git
cd Weather-App
```

2. Install dependencies:

```bash
npm install
```

## Run Locally

Start the development server:

```bash
npm run dev
```

Then open the local URL shown in the terminal (usually `http://localhost:5173`).

## Production Build

Create a production build:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

## Android App Build

This project includes Capacitor configuration for Android packaging.

To build the Android app:

```bash
npx cap add android
npx cap sync android
npx cap open android
```

If needed, you can also run:

```bash
npm run build
npx cap sync android
```

## Data Sources

This app uses:

- Open-Meteo Geocoding API for city search
- Open-Meteo Weather API for current and forecast weather data

No API key is required for the free tier used in this project.

## Notes

- Weather data depends on the Open-Meteo service availability.
- Some features such as geolocation require browser permission.
- This project is designed as a responsive PWA and hybrid app foundation.

## License

This project is currently unlicensed unless you explicitly add a license file.

## Author

Yugandhar2024

## Project Status

Active development / weather dashboard application ready for local use and Android packaging.
