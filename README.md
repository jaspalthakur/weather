# weather

Weather Dashboard Features

The page is built around a single search action that triggers a chain of API calls and UI updates.

    Search & Fetch Flow: When you submit a city name, the script first validates the input, then calls the Open-Meteo Geocoding API to find the city's coordinates. It uses those coordinates to fetch the current weather and a five-day forecast.

    Error & Loading States: The status area clearly shows "Loading weather..." while fetching, displays a specific error message if the city isn't found or the API fails, and confirms success with the city name.

    Dynamic Rendering: The current temperature, weather icon, and description are injected into the DOM, while the forecast section builds five individual cards (one per day) showing the high, low, and a weather icon.

    Data Persistence: The last searched city is saved in localStorage and automatically searched again when you reload the page, so your dashboard remembers your preference.
