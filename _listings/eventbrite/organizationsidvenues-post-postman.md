{
  "info": {
    "name": "Eventbrite Add Organizations  Venues",
    "_postman_id": "601967e7-8f24-4f12-bf3c-581047a73425",
    "description": "Creates new venue objects under an organization and returns it as venue.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "1c665037-e067-4473-abc6-ef71a2c756dd",
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
              "id": "8ee26ae1-08ba-46cd-917b-a94e763e5819"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "ade90e40-ecd1-4ef3-8b41-754c31a18320",
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
              "id": "905664e3-59e7-4036-bcbb-c53d58ccf94a"
            }
          ]
        }
      ]
    }
  ]
}