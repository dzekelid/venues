{
  "info": {
    "name": "Eventbrite Add Venues",
    "_postman_id": "c2e745ab-5941-4dd0-9acf-e29d7eebb650",
    "description": "Creates a new venue with associated address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "e213e3bd-a373-4f22-a0b7-cb8009062e2c",
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
              "id": "75679d09-b884-4582-8ba8-0b777b088ae2"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "fa6f3c25-5cd2-49a3-83c1-55c5635ea2dc",
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
              "id": "e6a3a8e7-a228-496e-ac03-4b0ca21a25df"
            }
          ]
        }
      ]
    },
    {
      "name": "Venues",
      "item": [
        {
          "id": "261eae68-bc37-4801-80c7-039c1654ba21",
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
              "id": "70953df6-7ba0-468f-b8e2-122b6a1816ba"
            }
          ]
        },
        {
          "id": "c51ca982-d336-4f35-9b96-357d4eb370c0",
          "name": "postVenues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "venues/:id/"
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
            "description": "Updates a venue and returns it as an object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64da1248-01f9-40a6-a1de-cde4a938c2de"
            }
          ]
        },
        {
          "id": "7fa947b2-bc24-4b56-8949-e62e41cc4403",
          "name": "postVenues1",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/venues/?venue.address.address_1=%7B%7D&venue.address.address_2=%7B%7D&venue.address.city=%7B%7D&venue.address.country=%7B%7D&venue.address.latitude=%7B%7D&venue.address.longitude=%7B%7D&venue.address.postal_code=%7B%7D&venue.address.region=%7B%7D&venue.age_restriction=%7B%7D&venue.capacity=%7B%7D&venue.google_place_id=%7B%7D&venue.name=%7B%7D&venue.organizer_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new venue with associated address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71b79d3f-3036-4d7e-9090-bc18edd5db74"
            }
          ]
        }
      ]
    }
  ]
}