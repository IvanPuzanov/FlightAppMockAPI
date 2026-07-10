# FlightApp Mock API

Static JSON mock data for the [FlightApp](https://github.com/IvanPuzanov/FlightApp) iOS demo.

This repository acts as a lightweight stand-in for a backend: the app can load flights, airports, airlines, and flight details from these files (for example via GitHub raw URLs).

## Contents

| Path | Description |
|---|---|
| [`airports.json`](airports.json) | Airports with IATA code, city, country, timezone, and coordinates |
| [`airlines.json`](airlines.json) | Airlines with IATA code, name, and logo URL |
| [`flights.json`](flights.json) | Flight list items (route, schedule, price, cabin class) |
| [`flight-details/`](flight-details) | Per-flight detail payloads (`FL1001.json` … `FL1029.json`) |

## Dataset

- **23** airports
- **18** airlines
- **29** flights (`FL1001`–`FL1029`)

## Example usage

Raw file URLs (replace `main` with a tag or commit SHA if you need a fixed version):

```text
https://raw.githubusercontent.com/IvanPuzanov/FlightAppMockAPI/main/airports.json
https://raw.githubusercontent.com/IvanPuzanov/FlightAppMockAPI/main/flights.json
https://raw.githubusercontent.com/IvanPuzanov/FlightAppMockAPI/main/airlines.json
https://raw.githubusercontent.com/IvanPuzanov/FlightAppMockAPI/main/flight-details/FL1001.json
```

## Related

- Demo app: [IvanPuzanov/FlightApp](https://github.com/IvanPuzanov/FlightApp)
