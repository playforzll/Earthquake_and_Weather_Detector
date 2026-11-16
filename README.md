
# Weather & Earthquake Detector 🌦️🌍

A Python-based weather and earthquake monitoring program that retrieves weather forecasts and earthquake information using public APIs.

## Features

- Weather forecasting for a specified city and country.
- Earthquake detection for a specified location and date.
- Earthquake risk classification based on magnitude.
- Weather alerts with safety recommendations.
- Location detection using OpenStreetMap.
- Retry option to perform multiple searches.

## APIs Used

- [OpenWeatherMap API](https://openweathermap.org/api) - Retrieves weather forecast information.
- [USGS Earthquake API](https://earthquake.usgs.gov/fdsnws/event/1/) - Retrieves earthquake information.
- [OpenStreetMap Nominatim API](https://nominatim.org/) - Converts locations into geographical coordinates.

## Earthquake Risk Classification

- 🟢 Low Risk: Magnitude ≤ 3
- 🟡 Medium Risk: Magnitude > 3 and < 6
- 🔴 High Risk: Magnitude ≥ 6

## Requirements

- Python 3.x
- Requests library

## Installation

1. Clone the repository:

```bash
git clone YOUR_REPOSITORY_URL
```

2. Navigate to the project directory:

```bash
cd YOUR_PROJECT_FOLDER
```

3. Install the required library:

```bash
pip install requests
```

## Usage

Run the Python file:

```bash
python3 main.py
```

Choose what you want to check:

```text
weather/earthquake
```

### Weather

Enter `weather`, followed by your country and city. The program will retrieve the weather forecast and display safety recommendations.

### Earthquake

Enter `earthquake`, followed by a location and date.

Use the following date format:

```text
YYYY-MM-DD
```

The program will display matching earthquakes, their locations, magnitudes, risk classifications, and occurrence times.

## Technologies Used

- Python
- Requests
- OpenWeatherMap API
- USGS Earthquake API
- OpenStreetMap Nominatim

## Notes

- An active internet connection is required.
- Weather information depends on the OpenWeatherMap API.
- Earthquake information is provided by the USGS.
- Risk classifications are simplified magnitude-based labels and are not official safety assessments.

## Author

Developed as a Python project to explore API integration, data retrieval, and environmental monitoring.

## LICENSE

This project is licensed under the GNU General Public License v3.0, if you choose GPL-3.0. See the LICENSE file for details.
