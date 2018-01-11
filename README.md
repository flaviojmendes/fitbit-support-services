## Fitbit Support Services

This service works in order to make easier the life of a Fitbit Developer.

For now it is supporting weather retrievals for DarkSky and OpenWeatherMap API.


### How to start

To start the service simply execute:

```
./gradlew build && ./gradlew buildDocker && docker-compose up -d
```

### How to use

Fist you need to add some API Keys:

```
HTTP POST
http://{domain}/apiKey/{DARKSKY|OPENWEATHER}/

BODY
{key1},{key2},...,{keyN}

```

To retrieve weather:

```
HTTP GET
http://{domain}/weather/{DARKSKY|OPENWEATHER}/{latitude}/{longitude}/

```