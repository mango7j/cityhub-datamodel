# WeatherForecast

**Note: Notification text here.

## Description 

Model description here. Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...

## Data model 

A JSON Schema corresponding to this data model can be found 
[here](https://github.com/IoTKETI/datahub_data_modeling/raw/master/1%EC%B0%A8%20PoC/1.OffStreetParking.json)

- `id` : Entity's unique identifier.

- `type`: Entity type. It must be equal to 'OffStreetParking'.

T.B.W

## Example

### Normalized Example 

```json
{
   "@context": [
      "http://uri.etsi.org/ngsi-ld/core-context.jsonld",
      "http://cityhub.kr/ngsi-ld/weather.jsonld"
   ],
   "id": "urn:datahub:WeatherForecast:6279",
   "type": "WeatherForecast",
   "createdAt": "2018-11-15T20:10:00,000+09:00",
   "modifiedAt": "2018-11-15T20:10:00,000+09:00",
   "location": {
      "type": "GeoProperty",
      "value": {
         "type": "Point",
         "coordinates": [
            127.1293735,
            37.4114423
         ]
      }
   },
   "address": {
      "type": "Property",
      "value": {
         "addressCountry": "KR",
         "addressRegion": "Gyeonggi-do",
         "addressLocality": "Seongnam-si",
         "streetAddress": "8th Seungin-ro",
         "addressTown": "Yatap-dong"
      }
   },
   "weatherPrediction": {
      "type": "Property",
      "value": [
         {
            "temperature": 10.1,
            "lowestTemperature": -3.0,
            "highestTemperature": 7.0,
            "windSpeed": 0.2,
            "humidity": 68,
            "rainfall": 10,
            "rainfallProbability": 60,
            "rainType": "비",
            "snowfall": 0,
            "predictedAt": "2019-06-08T06:00:00,000+09:00"
         },
         {
            "temperature": 14.1,
            "lowestTemperature": -3.0,
            "highestTemperature": 7.0,
            "windSpeed": 0.3,
            "humidity": 65,
            "rainfall": 20,
            "rainfallProbability": 60,
            "rainType": "비",
            "snowfall": 0,
            "predictedAt": "2019-06-08T09:00:00,000+09:00"
         }
      ],
      "observedAt": "2018-11-15T20:09:55,000+09:00"
   }
}
```

### key-value pairs Example 

T.B.W 

## Use it with a real service 

The model has been defined to support different scenarios inside
[CityhubSDK](http://city-hub.kr/services) project.

## Open Issues

T.B.W