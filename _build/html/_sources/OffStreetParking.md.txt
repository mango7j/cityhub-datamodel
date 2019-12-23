# OffStreetParking 

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
      "http://cityhub.kr/ngsi-ld/parking.jsonld"
   ],
   "id": "urn:datahub:OffStreetParking:yatap_01",
   "type": "OffStreetParking",
   "createdAt": "2018-11-15T20:10:00,000+09:00",
   "modifiedAt": "2018-11-15T20:10:00,000+09:00",
   "name": {
      "type": "Property",
      "value": "yatap_01"
   },
   "location": {
      "type": "GeoProperty",
      "value": {
         "type": "Point",
         "coordinates": [
            127.1293735,
            37.4114424
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
   "locationTag": {
      "type": "Property",
      "value": "commercial"
   },
   "category": {
      "type": "Property",
      "value": [
         "public",
         "feeCharged"
      ]
   },
   "paymentAccepted": {
      "type": "Property",
      "value": [
         "Cash",
         "Credit Card"
      ]
   },
   "priceRate": {
      "type": "Property",
      "value": "최초 30분 무료 free, 이후 10분당 500원"
   },
   "priceCurrency": {
      "type": "Property",
      "value": [
         "KRW"
      ]
   },
   "image": {
      "type": "Property",
      "value": "https://raw.githubusercontent.com/IoTKETI/image/master/City_hub_yt_lot_1.jpg"
   },
   "totalSpotNumber": {
      "type": "Property",
      "value": 110
   },
   "availableSpotNumber": {
      "type": "Property",
      "value": 40,
      "observedAt": "2018-11-15T20:09:55,000+09:00"
   },
   "maximumAllowedHeight": {
      "type": "Property",
      "value": 2.2
   },
   "openingHours": {
      "type": "Property",
      "value": [
         "Mo-Su 00:00-24:00"
      ]
   },
   "contactPoint": {
      "type": "Property",
      "value": {
         "telephone": "031-000-0000",
         "email": "parking@seongnam.kr",
         "contactType": "City-hall"
      }
   },
   "status": {
      "type": "Property",
      "value": [
         "open",
         "spaceAvailable"
      ]
   },
   "refParkingSpots": {
      "type": "Property",
      "value": [
         "urn:datahub:ParkingSpot:yatap_540",
         "urn:datahub:ParkingSpot:yatap_541"
      ]
   },
   "congestionIndexPrediction": {
      "type": "Property",
      "value": [
         {
            "index": 2,
            "predictedAt": "2019-06-14T11:00:00,000+09:00"
         },
         {
            "index": 5,
            "predictedAt": "2019-06-14T12:00:00,000+09:00"
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