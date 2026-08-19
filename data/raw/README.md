# Data Setup

Raw source data are intentionally **not committed** to this repository.

## 1. Capital Bikeshare trip data

Source:

https://capitalbikeshare.com/system-data

Download the **2025 Capital Bikeshare trip-history CSV files** and place the extracted CSV files in:

```text
data/raw/
```

The notebook searches for filenames containing:

```text
capitalbikeshare-tripdata
```

Required columns include:

```text
ride_id
started_at
ended_at
start_station_name
end_station_name
```

## 2. Washington, DC weather data

The original project used a 2025 Washington, DC daily weather export from Visual Crossing:

https://www.visualcrossing.com/weather-history/

Save the file as:

```text
data/raw/DC_weather_2025.csv
```

The final modeling notebook expects these columns:

```text
datetime
temp
precip
windspeed
uvindex
icon
```

## Why the raw files are excluded

Capital Bikeshare trip-history data are large, and source datasets are better obtained directly from their authoritative providers. The repository therefore contains code, results, and visualizations while `.gitignore` keeps raw data out of version control.
