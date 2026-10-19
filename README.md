# Travel Weather & Country Info Tool

A simple Python command-line utility that fetches real-time weather details for any city and links them to comprehensive national information using API chaining. 

## How It Works

1. **Weather Fetching:** Takes user input for a city name and queries the **OpenWeatherMap API** to extract current temperature, atmospheric conditions, humidity, and wind speed.
2. **API Chaining:** Automatically extracts the country code (e.g., `KE` for Nairobi) from the weather response payload and feeds it straight into the **REST Countries API** to pull regional data, population stats, and official currencies.
3. **Local Caching:** Automatically saves raw JSON responses locally (e.g., `nairobi_weather.json`) to prevent hitting API rate limits during testing and development.

---

## Quick Start Guide

### Prerequisites
Make sure you have Python installed along with the required libraries:
```bash
pip install requests python-dotenv