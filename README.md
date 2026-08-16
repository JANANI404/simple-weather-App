# simple-weather-App
A simple weather app built with vanilla HTML, CSS, and JavaScript. Search any city to get real-time temperature, weather description, and conditions using the OpenWeatherMap API.

Weather App

A simple, responsive weather app that lets users search for any city and instantly view current weather conditions — including temperature, sky description, and a weather icon — powered by the OpenWeatherMap API.

Built as a hands-on project to practice working with real-world APIs, asynchronous JavaScript, and DOM manipulation using nothing but vanilla HTML, CSS, and JS.

Features
Search current weather by city name
Displays temperature (°C), weather description, and a matching icon
Handles empty input and invalid city names gracefully
Built with async/await and the Fetch API — no page reloads
Fully responsive layout using CSS Flexbox

Tech Stack
HTML — page structure
CSS — Flexbox-based layout and styling
JavaScript (Vanilla) — API calls, async/await, DOM manipulation
OpenWeatherMap API — geocoding + current weather data

No frameworks, libraries, or build tools — just the fundamentals.

How It Works
The user types a city name and hits Search.
The app calls OpenWeatherMap's Geocoding API to convert the city name into latitude/longitude coordinates.
Those coordinates are passed to OpenWeatherMap's Current Weather API to fetch live weather data.
The result — temperature, description, and icon — is rendered dynamically on the page.

Getting Started
Prerequisites
A free OpenWeatherMap account and API key
A code editor (e.g., VS Code)
A local server extension like Live Server (recommended, since this project uses fetch()

Setup
Clone the repository
   git clone https://github.com/your-username/weather-app.git
   cd weather-app
Add your API key Open script.js and replace the placeholder with your own OpenWeatherMap API key:
javascript
   const apiKey = "YOUR_API_KEY_HERE";

 Note: New OpenWeatherMap API keys can take up to a couple of hours to activate after signup.

Run it locally Open index.html with a local server (e.g., right-click → "Open with Live Server" in VS Code), or simply open the file directly in your browser.
Search for a city and see the weather appear!

Project Structure
weather-app/
├── index.html      # Page structure
├── styles.css       # Styling and layout
├── script.js        # API calls and app logic
└── README.md

A Note on API Keys

This project uses a client-side API key for simplicity, meaning it's visible in the browser's network tab and page source. This is fine for a free-tier learning project, but not recommended for production apps — a real-world app would route API calls through a backend server to keep the key hidden.

If you fork or clone this repo, make sure to use your own API key rather than any key that may appear in commit history.

Potential Improvements
 Add a 5-day forecast view
 Show additional data (humidity, wind speed, "feels like" temperature)
 Add a loading indicator while fetching data
 Let users toggle between °C and °F
 Handle rapid repeated searches more gracefully (avoid race conditions between requests)
 Add geolocation support ("Use my current location")

License

This project is open source and available under the MIT License.

🙏 Acknowledgments
Weather data provided by OpenWeatherMap
Project structure inspired by the Codédex weather app tutorial
