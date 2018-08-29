{
  "info": {
    "name": "Foursquare Get Venues Categories",
    "_postman_id": "4d1046bf-d3f5-4dba-a0ac-91c8c8bc5546",
    "description": "/venues/add",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "286b0377-3cac-4bae-b436-952902be9dcf",
          "name": "eventsevent-id",
          "request": {
            "url": "http://api.foursquare.com/v2/events/categories?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/{EVENT_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4913b905-b8ce-4065-a1dc-149100ed8836"
            }
          ]
        }
      ]
    },
    {
      "name": "Venues",
      "item": [
        {
          "id": "5297b640-9294-4197-b3a0-e1372e42db70",
          "name": "venuesadd",
          "request": {
            "url": "http://api.foursquare.com/v2/venues/categories?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venues/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "821020f9-8287-46d8-9275-62e779d96f19"
            }
          ]
        }
      ]
    }
  ]
}