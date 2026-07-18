# FlightApp Mock API

Static JSON mock data for the [FlightApp](https://github.com/IvanPuzanov/FlightApp) iOS demo.

This repository acts as a lightweight stand-in for a backend: the app can load flights, airports, airlines, and flight details from these files (for example via GitHub raw URLs).

## Contents

| Path | Description |
|---|---|
| [`airports.json`](airports.json) | Airports with `id`, `iata`, name, city, country, `latitude`/`longitude`, timezone, and inbound `flightIds` (only airports that appear as a flight destination) |
| [`airlines.json`](airlines.json) | Airlines with IATA code, name, and logo URL |
| [`flights.json`](flights.json) | Flight list items: airline, airports, ISO-8601 schedule, price, included baggage, optional selling `status` |
| [`flight-details/`](flight-details) | Per-flight details: airline, ISO-8601 schedule, and available `fares` (baggage, cancellation, changes, amenities) |

## Dataset

- **18** airports (destinations with inbound flights)
- **18** airlines
- **29** flights (IDs match airline flight numbers, e.g. `OS101`, `TK64`, `LH400`)

## Example usage

Raw file URLs (replace `main` with a tag or commit SHA if you need a fixed version):

```text
https://raw.githubusercontent.com/IvanPuzanov/FlightAppMockAPI/main/airports.json
https://raw.githubusercontent.com/IvanPuzanov/FlightAppMockAPI/main/flights.json
https://raw.githubusercontent.com/IvanPuzanov/FlightAppMockAPI/main/airlines.json
https://raw.githubusercontent.com/IvanPuzanov/FlightAppMockAPI/main/flight-details/OS101.json
```

## Related

- Demo app: [IvanPuzanov/FlightApp](https://github.com/IvanPuzanov/FlightApp)
