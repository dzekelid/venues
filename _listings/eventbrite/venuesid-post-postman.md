{
  "info": {
    "name": "Eventbrite Add Venues",
    "_postman_id": "36f7cd82-7547-4278-8b94-4cb7599a65d4",
    "description": "Updates a venue and returns it as an object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "d9617f51-69eb-4c39-a63d-1b1cf6be817e",
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
              "id": "47ad0000-d19f-42f3-be2b-84bd81854db7"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "2f29f764-4d06-4a88-9781-ca3ba6d9aaba",
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
              "id": "2ba15555-2be7-400d-bdfa-185c5fdf77cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Venues",
      "item": [
        {
          "id": "a12d3426-c7f6-4162-983f-7879434357bc",
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
              "id": "94baa4b7-e3da-41bc-a731-7ae36e51f25b"
            }
          ]
        },
        {
          "id": "e02cd623-f1c2-44a1-bf9d-a27163a531f9",
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
              "id": "69bc97ac-de6e-44c1-b09b-30dfe4b69db5"
            }
          ]
        }
      ]
    }
  ]
}