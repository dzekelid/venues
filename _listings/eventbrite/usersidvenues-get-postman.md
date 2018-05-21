{
  "info": {
    "name": "Eventbrite Get Users  Venues",
    "_postman_id": "7e83b606-33c7-4a7f-a80a-b4b002cd0b1d",
    "description": "Returns a paginated response of venue objects that are owned by the user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "58bf484f-102f-45a2-afd7-b42fe02b2ebf",
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
              "id": "2aea0fca-19f0-4359-b8ed-cf4f516a8207"
            }
          ]
        }
      ]
    }
  ]
}