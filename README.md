# Airport API

## Documentation

### `[GET] /airlines`

```json
[
  {
    "id": "aeromexico",
    "name": "Aeromexico",
    "code": {
      "iata": "AM",
      "icao": "AMX"
    },
    "logotype": {
      "url": "http://upload.wikimedia.org/wikipedia/en/b/bc/AeroM%C3%A9xico_Logo.svg",
      "source": "https://en.wikipedia.org/wiki/Aerom%C3%A9xico"
    }
  },
  {
    "id": "iberia",
    "name": "Iberia",
    "code": {
      "iata": "IB",
      "icao": "IBE"
    },
    "logotype": {
      "url": "http://upload.wikimedia.org/wikipedia/en/2/23/American_Airlines_logo_2013.svg",
      "source": "https://en.wikipedia.org/wiki/Iberia_%28airline%29"
    }
  },
  ...
]
```

### `[GET] /schedules`

```json
[
  {
    "id": "a1b2c3d9e8f7",
    "flightId": "AA-432",
    "status": "On time",
    "airline": {
      "id": "american-airlines",
      "name": "American Airlines",
      "code": {
        "iata": "AA",
        "icao": "AAL"
      },
      "logotype": {
        "url": "http://upload.wikimedia.org/wikipedia/commons/e/e6/Iberia_%282013%29.svg",
        "source": "https://en.wikipedia.org/wiki/American_Airlines"
      }
    },
    "departure": {
      "location": {
        "country": {
          "name": "Mexico",
          "code": "MX"
        },
        "city": "Guadalajara",
        "airportCode": "GDL"
      },
      "dateTime": "2015-09-24T11:59Z",
      "terminal": "1",
      "gate": "A-1"
    },
    "arrival": {
      "location": {
        "country": {
          "name": "United States",
          "code": "US"
        },
        "city": "San Francisco",
        "airportCode": "SFO"
      },
      "dateTime": "2015-09-25T01:25Z",
      "terminal": "2",
      "gate": "B-3"
    }
  },
  ...
]
```

## Available mock data

### Airlines

| Name              | IATA code | ICAO code | Logo | Source |
|-------------------|-----------|-----------|:----:|--------|
| Aeromexico        | AM        | AMX       | ![Aeromexico logo](http://upload.wikimedia.org/wikipedia/en/b/bc/AeroM%C3%A9xico_Logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Aerom%C3%A9xico) |
| Air France        | AF        | AFR       | ![Air France logo](http://upload.wikimedia.org/wikipedia/commons/4/44/Air_France_Logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Air_France) |
| Alitalia          | AZ        | AZA       | ![Alitalia logo](http://upload.wikimedia.org/wikipedia/en/f/f1/Alitalia_logo_2015.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Alitalia) |
| American Airlines | AA        | AAL       | ![American Airlines logo](http://upload.wikimedia.org/wikipedia/en/2/23/American_Airlines_logo_2013.svg) | [Wikipedia](https://en.wikipedia.org/wiki/American_Airlines) |
| Aviacsa           | 6A        | CHP       | ![Aviacsa logo](http://upload.wikimedia.org/wikipedia/commons/5/55/Aviacsa_Logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Aviacsa) |
| British Airways   | BA        | BAW       | ![British Airways logo](http://upload.wikimedia.org/wikipedia/en/4/42/British_Airways_Logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/British_Airways) |
| Delta Air Lines   | DL        | DAL       | ![Delta Air Lines logo](http://upload.wikimedia.org/wikipedia/commons/d/d1/Delta_logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Delta_Air_Lines) |
| Emirates          | EK        | UAE       | ![Emirates logo](http://upload.wikimedia.org/wikipedia/commons/d/d0/Emirates_logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Emirates_%28airline%29) |
| Iberia            | IB        | IBE       | ![Iberia logo](http://upload.wikimedia.org/wikipedia/commons/e/e6/Iberia_%282013%29.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Iberia_%28airline%29) |
| KLM               | KL        | KLM       | ![KLM logo](http://upload.wikimedia.org/wikipedia/commons/c/c7/KLM_logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/KLM) |
| Lufthansa         | LH        | DHL       | ![Lufthansa logo](http://upload.wikimedia.org/wikipedia/en/5/54/Lufthansa_Logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Lufthansa) |
| Oceanic Airlines  | -         | -         | ![Oceanic Airlines logo](http://upload.wikimedia.org/wikipedia/en/5/51/Oceanic.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Oceanic_Airlines) |
| United Airlines   | UA        | UAL       | ![United Airlines logo](http://upload.wikimedia.org/wikipedia/en/e/e0/United_Airlines_Logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/United_Airlines) |
| Virgin America    | VX        | VRD       | ![Virgin America logo](http://upload.wikimedia.org/wikipedia/en/7/78/Vx-logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Virgin_America) |
| Volaris           | Y4        | VOI       | ![Volaris logo](http://upload.wikimedia.org/wikipedia/en/b/b2/Volaris_logo.svg) | [Wikipedia](https://en.wikipedia.org/wiki/Volaris) |
