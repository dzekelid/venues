{
  "info": {
    "name": "Eventbrite Get Venues  Events",
    "_postman_id": "a7c2fd03-3d89-416f-9598-c33300b2982a",
    "description": "Returns events of a given venue.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "e01c3039-6cab-449a-be66-694e059f51af",
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
              "id": "f5e56ec5-4f37-4bac-a9fc-55054320874c"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "6ce0807f-cfed-4014-93c5-a8e19949b94b",
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
              "id": "bd6d2a0c-3bcf-4427-8a59-93db3d3e12bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Venues",
      "item": [
        {
          "id": "f4cd1422-5197-4b42-92d5-480ba1655c00",
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
              "id": "41c581de-fc04-471d-9445-cdfde7e399b7"
            }
          ]
        },
        {
          "id": "1cdef782-5d5e-4af6-9bcf-67b3acc086ad",
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
              "id": "5f2c2356-6405-49f3-95dd-120e7ec06f1e"
            }
          ]
        },
        {
          "id": "6792e4b7-cb22-4aa0-b3a5-41e494c53262",
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
              "id": "e71a2efc-f60c-4233-8808-192dea6f20f3"
            }
          ]
        },
        {
          "id": "dde8f56a-236c-481f-ae2c-5a3646fea226",
          "name": "getVenuesEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "venues/:id/events/"
              ],
              "query": [
                {
                  "key": "only_public",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order_by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date.range_end",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date.range_start",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "status",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns events of a given venue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb1abb96-5311-48e1-9bc7-7c89dde6d19e"
            }
          ]
        }
      ]
    }
  ]
}