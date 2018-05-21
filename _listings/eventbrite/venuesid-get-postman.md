{
  "info": {
    "name": "Eventbrite Get Venues",
    "_postman_id": "0acd2f47-da2b-460b-83ca-6f52058a5fc6",
    "description": "Returns a venue object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "0eea1e4b-9bb3-4c26-add9-2bee5d1c2757",
          "name": "getUsersVenues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "users/:id/venues/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated response of venue objects that are owned by the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b010b6c3-f1b2-4493-a132-b8b56711281d"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "fb4e8877-ed58-4ff1-9fd4-2226a0f41781",
          "name": "postOrganizationsVenues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "organizations/:id/venues/"
              ],
              "query": [
                {
                  "key": "venue.address.address_1",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.address.address_2",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.address.city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.address.country",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.address.latitude",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.address.longitude",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.address.postal_code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.address.region",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.age_restriction",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.capacity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.google_place_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venue.organizer_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates new venue objects under an organization and returns it as venue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aedbdc51-def6-4d3e-b990-7540caa383e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Venues",
      "item": [
        {
          "id": "3236c15a-8f64-4335-b9c7-7c013192f4b7",
          "name": "getVenues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "venues/:id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a venue object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c5401dd-f6fd-4aa3-a697-89303115df81"
            }
          ]
        }
      ]
    }
  ]
}