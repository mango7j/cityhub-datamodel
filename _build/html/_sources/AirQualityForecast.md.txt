# AirQualityForecast

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
      "http://cityhub.kr/ngsi-ld/airquality.jsonld"
   ],
   "id": "urn:datahub:AirQualityForecast:6831",
   "type": "AirQualityForecast",
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
   "airQualityPrediction": {
      "type": "Property",
      "value": [
         {
            "so2": 0.007,
            "co": 0.9,
            "o3": 0.03,
            "no2": 0.08,
            "pm10": 33,
            "pm25": 22,
            "predictedAt": "2019-06-14T05:00:00,000+09:00"
         },
         {
            "so2": 0.009,
            "co": 0.7,
            "o3": 0.02,
            "no2": 0.05,
            "pm10": 23,
            "pm25": 12,
            "predictedAt": "2019-06-14T06:00:00,000+09:00"
         }
      ],
      "observedAt": "2018-11-15T20:09:55,000+09:00"
   },
   "airQualityIndexPrediction": {
      "type": "Property",
      "value": [
         {
            "totalIndex": 20,
            "totalCategory": "좋음",
            "so2Category": "좋음",
            "coCategory": "좋음",
            "o3Category": "좋음",
            "no2Category": "좋음",
            "pm10Category": "좋음",
            "pm25Category": "좋음",
            "predictedAt": "2019-06-14T05:00:00,000+09:00"
         },
         {
            "totalIndex": 20,
            "totalCategory": "좋음",
            "so2Category": "좋음",
            "coCategory": "좋음",
            "o3Category": "좋음",
            "no2Category": "좋음",
            "pm10Category": "좋음",
            "pm25Category": "좋음",
            "predictedAt": "2019-06-14T06:00:00,000+09:00"
         }
      ],
      "observedAt": "2018-11-15T20:09:55,000+09:00"
   },
   "indexRef": {
      "type": "Property",
      "value": "https://www.airkorea.or.kr/web/khaiInfo?pMENU_NO=129"
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