# ParkingSpot

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
   "id": "urn:datahub:ParkingSpot:yatap_540",
   "type": "ParkingSpot",
   "createdAt": "2018-11-15T20:10:00,000+09:00",
   "modifiedAt": "2018-11-15T20:10:00,000+09:00",
   "name": {
      "type": "Property",
      "value": "spot_001"
   },
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
   "category": {
      "type": "Property",
      "value": [
         "forDisabled"
      ]
   },
   "width": {
      "type": "Property",
      "value": 2.5
   },
   "length": {
      "type": "Property",
      "value": 5.1
   },
   "status": {
      "type": "Property",
      "value": "free",
      "observedAt": "2018-11-15T20:09:55,000+09:00"
   },
   "refParkingLot": {
      "type": "Property",
      "value": "urn:ngsi-ld:OffStreetParking:5038"
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