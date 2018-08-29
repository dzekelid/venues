{
  "info": {
    "name": "Foursquare Get Venues",
    "_postman_id": "f0b5ce7d-9ae3-496b-b795-0c13d8a0c6c4",
    "description": "/users/self/update",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaigns",
      "item": [
        {
          "id": "2b83461a-3db5-47d4-b24f-14a4c83b4262",
          "name": "campaignscampaign-id",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/add?campaignId=%7B%7D&endAt=%7B%7D&groupId=%7B%7D&specialId=%7B%7D&startAt=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76a29750-3653-4d69-a8f4-1ae889fbacfa"
            }
          ]
        },
        {
          "id": "e6e4c68a-74cf-4242-959c-2167f4083ecf",
          "name": "campaignsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/list?groupId=%7B%7D&specialId=%7B%7D&status=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed19f0c0-9902-4aef-bb4d-1a6c3347f6f1"
            }
          ]
        },
        {
          "id": "a3c7ace8-7a55-47eb-ad2e-08dd760847ac",
          "name": "specialsspecial-idretire",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}/retire"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71494c6e-8b97-40fa-9f25-486f09d560a8"
            }
          ]
        },
        {
          "id": "078c4b72-7d2f-4dc8-a0d0-a992fcaaa6ca",
          "name": "campaignscampaign-idtimeseries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/delete"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/timeseries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35aa8e8f-417b-455e-9172-287d58acacb8"
            }
          ]
        },
        {
          "id": "148a8a77-08b1-4859-9819-52b20cf47238",
          "name": "campaignscampaign-iddelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/end"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/delete"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b735ba1-a071-410f-a099-46868a63c392"
            }
          ]
        },
        {
          "id": "c8f2127b-a613-406c-9e6b-ed031e73d976",
          "name": "campaignscampaign-idend",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/start"
              ],
              "query": [
                {
                  "key": "startAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/end"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b527d2c-8167-4daa-a9aa-8d7e3d31d643"
            }
          ]
        },
        {
          "id": "b87fd7f6-9768-46f4-86f1-6ca9f1359c6d",
          "name": "campaignslist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/timeseries"
              ],
              "query": [
                {
                  "key": "endAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71d06f26-2922-407f-9273-7a91d9e3c682"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkins",
      "item": [
        {
          "id": "fb20f3bf-780b-4139-94f6-2a7414588844",
          "name": "checkinscheckin-id",
          "request": {
            "url": "http://api.foursquare.com/v2/checkins/add?alt=%7B%7D&altAcc=%7B%7D&broadcast=%7B%7D&eventId=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&shout=%7B%7D&v=%7B%7D&venue=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "330d4cce-da85-4ac5-a166-2d6c7ff3cbf1"
            }
          ]
        },
        {
          "id": "9ea400cf-e259-464a-9cda-1957aadef80c",
          "name": "checkinsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/checkins/recent?afterTimestamp=%7B%7D&limit=%7B%7D&ll=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70852e24-9835-4b70-b09c-21f46b53b572"
            }
          ]
        },
        {
          "id": "f452214b-1310-4024-8917-63eb559375f3",
          "name": "venuegroupsgroup-idremovevenue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID"
              ],
              "query": [
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venuegroups/{GROUP_ID}/removevenue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a4613e7-2c0b-4c1b-af0c-d2a264ffbd0a"
            }
          ]
        },
        {
          "id": "e54d97d2-d445-48c6-8e11-e59463525a23",
          "name": "checkinsrecent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID/addcomment"
              ],
              "query": [
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/recent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "031117ca-437a-46dd-aad8-989141966b0a"
            }
          ]
        },
        {
          "id": "d154ac4f-a4e3-4fb4-b565-a488492cef6d",
          "name": "checkinscheckin-idaddcomment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID/deletecomment"
              ],
              "query": [
                {
                  "key": "commentId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}/addcomment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6d3a8c8-13e5-4a9d-803c-91315ccfaa8a"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "01ab5f11-97db-4709-adc3-fc14caf26544",
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
              "id": "2a506628-c12c-4538-898e-e9bd3da055a6"
            }
          ]
        },
        {
          "id": "29a6246e-b300-464e-a4df-1b557d615b04",
          "name": "eventscategories",
          "request": {
            "url": "http://api.foursquare.com/v2/events/search?domain=%7B%7D&eventId=%7B%7D&participantId=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd80247d-0469-43ef-bb70-1bc3a5447378"
            }
          ]
        },
        {
          "id": "12599956-ee7e-4f2d-8a34-c0e6bc7ba489",
          "name": "campaignscampaign-idstart",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "events/:EVENT_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "EVENT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/start"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb41ca4e-45b2-4d74-be8f-06688807afbb"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "4f761e70-c9e7-4259-b6a7-3250262269c8",
          "name": "listslist-id",
          "request": {
            "url": "http://api.foursquare.com/v2/lists/add?collaborative=%7B%7D&description=%7B%7D&name=%7B%7D&photoId=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bee3c89b-a067-4c8e-89ef-5ab5f00db987"
            }
          ]
        },
        {
          "id": "88ef0cfe-0a88-45bb-a64a-9843e9d2a012",
          "name": "tipstip-idunmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/unmark"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02a5e984-a62a-43fa-b12d-9443cc41b951"
            }
          ]
        },
        {
          "id": "9a17a959-4577-4894-880e-98c0e9010a76",
          "name": "listslist-idsuggestvenues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/additem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "listId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tipId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggestvenues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2cf88065-6dea-4a5b-841f-b6e9a663617a"
            }
          ]
        },
        {
          "id": "fb6bfe49-b40d-4f46-8161-b706f2bf0513",
          "name": "listslist-idadditem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/deleteitem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/additem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf683e84-a6a6-4055-b361-ba1b790edb6e"
            }
          ]
        },
        {
          "id": "2b3e3ece-fd6e-4359-ab3f-37ca8cd5d95a",
          "name": "listslist-iddeleteitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/follow"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/deleteitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4d5fb41-3296-46f4-a5ba-871b78e76289"
            }
          ]
        },
        {
          "id": "b6789285-734c-44a6-b264-e723e79f1563",
          "name": "listsadd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/followers"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a55b61e5-ba16-42b9-bdcc-20e76576f203"
            }
          ]
        },
        {
          "id": "fb02b62e-454f-4f98-9bec-ec21e758d4b3",
          "name": "listslist-idfollow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/moveitem"
              ],
              "query": [
                {
                  "key": "afterId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "beforeId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/follow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6043b75e-00aa-40ee-b380-27a0b9e992c8"
            }
          ]
        },
        {
          "id": "c401097e-7493-47f0-93e1-c17cc570ef21",
          "name": "listslist-idmoveitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/share"
              ],
              "query": [
                {
                  "key": "broadcast",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/moveitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b962e84-db39-4226-9008-995daab220cc"
            }
          ]
        },
        {
          "id": "94469fb9-b293-4919-b261-8c6f9d8bb94c",
          "name": "listslist-idfollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggestphoto"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/followers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0f3f62c-c3bf-464b-b068-4e542c26d6fe"
            }
          ]
        },
        {
          "id": "fc38fdb9-909a-46ce-b5e1-82ff6d59b7d2",
          "name": "listslist-idsuggestphoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggesttip"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggestphoto"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f574b30d-818a-4203-a9a0-fe83bb87654b"
            }
          ]
        },
        {
          "id": "5d65b15b-438d-4a53-a2dc-44f94ffb74bc",
          "name": "listslist-idsuggesttip",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggestvenues"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggesttip"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "274f2fc6-f860-4788-9b54-dbf382232f3f"
            }
          ]
        },
        {
          "id": "19997e7f-86af-453a-b633-14b8fcf445ba",
          "name": "listslist-idshare",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/unfollow"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/share"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c72bd53e-86a2-448d-b58c-4b3e8e49d48d"
            }
          ]
        },
        {
          "id": "1fdbc551-4fc7-4e8c-ae23-fae9420f0266",
          "name": "listslist-idunfollow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/update"
              ],
              "query": [
                {
                  "key": "collaborative",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "photoId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/unfollow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec5d0276-8b8e-4116-a087-0057df1c2ab2"
            }
          ]
        },
        {
          "id": "b9b1aaf4-3df3-4c1e-a8bd-0885d72bae3c",
          "name": "listslist-idupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/updateitem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "photoId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tipId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d981dfa-3604-41ef-bb3d-1377fd022c8d"
            }
          ]
        }
      ]
    },
    {
      "name": "Multi",
      "item": [
        {
          "id": "60d7b288-08c5-46f1-836e-45eaa023d6d8",
          "name": "pagespage-idvenues",
          "request": {
            "url": "http://api.foursquare.com/v2/multi?requests=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/{PAGE_ID}/venues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ea444c1-b7f2-4921-900e-579eed5c0777"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "e5c5b9c6-ee76-4518-b962-4c012ea4ca2e",
          "name": "pagespage-id",
          "request": {
            "url": "http://api.foursquare.com/v2/pages/search?fbid=%7B%7D&name=%7B%7D&twitter=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/{PAGE_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aff4c8cf-a235-4f4e-a839-c6715ba78abd"
            }
          ]
        },
        {
          "id": "1680b528-8205-46f9-8c13-07f75b34245b",
          "name": "eventssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "pages/:PAGE_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PAGE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad8d409e-6dd6-4456-b135-93a2c310c1f3"
            }
          ]
        },
        {
          "id": "e4441f7f-f01c-4db5-8596-42d305bbc6ed",
          "name": "pagessearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "pages/:PAGE_ID/venues"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ll",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ne",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "radius",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sw",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PAGE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a699e4ff-5630-4376-86e2-4b7644ceecbd"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "1dcb2961-922d-41ad-bbcc-90779ea8dc7e",
          "name": "photosphoto-id",
          "request": {
            "url": "http://api.foursquare.com/v2/photos/add?alt=%7B%7D&altAcc=%7B%7D&broadcast=%7B%7D&checkinId=%7B%7D&Content-Type=%7B%7D&image=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&public=%7B%7D&tipId=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/photos/{PHOTO_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ebe1b41-a751-477f-80b6-a1e4f4573d2a"
            }
          ]
        },
        {
          "id": "364c8522-96dc-4548-a775-d4aa589b0827",
          "name": "updatesmarknotificationsread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "photos/:PHOTO_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PHOTO_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/updates/marknotificationsread"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "699bfc45-cc4c-42f6-aebb-86c6fde870ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Settings",
      "item": [
        {
          "id": "47aabe08-d624-46b2-96ba-b3d402b36a5e",
          "name": "settingssetting-id",
          "request": {
            "url": "http://api.foursquare.com/v2/settings/all?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/{SETTING_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2ee396a-7fdb-45df-83b6-eee620d61a60"
            }
          ]
        },
        {
          "id": "961a5485-1f8e-4724-ab80-f4dda13f4218",
          "name": "photosadd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "settings/:SETTING_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SETTING_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/photos/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1978a06c-8933-40d9-b0f7-af929524e9b2"
            }
          ]
        },
        {
          "id": "eee98e03-7ce4-4374-9111-b61a79a2cd94",
          "name": "settingsall",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "settings/:SETTING_ID/set"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SETTING_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "778727ee-8de1-4b5c-a85c-6658409a71da"
            }
          ]
        }
      ]
    },
    {
      "name": "Specials",
      "item": [
        {
          "id": "16427e7c-2e27-4584-b413-118e2d296bce",
          "name": "specialsspecial-id",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/add?cost=%7B%7D&count1=%7B%7D&count2=%7B%7D&count3=%7B%7D&finePrint=%7B%7D&name=%7B%7D&offerId=%7B%7D&text=%7B%7D&type=%7B%7D&unlockedText=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2d4c528-795a-476b-bd17-d1d18615c0e8"
            }
          ]
        },
        {
          "id": "472a7fce-04fe-4830-90a4-219ebd0d3685",
          "name": "specialsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/list?status=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5881678-304e-4724-a71b-2c5ea702c220"
            }
          ]
        },
        {
          "id": "2924ae5b-935b-48d8-844c-370fb3f72409",
          "name": "specialslist",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/search?alt=%7B%7D&altAcc=%7B%7D&limit=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&radius=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69c59a4b-70dd-4549-9d5d-3ebbae8acee0"
            }
          ]
        },
        {
          "id": "72e7576d-c682-429f-bdb8-e79ff5f3a745",
          "name": "specialsspecial-idconfiguration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:ID/flag"
              ],
              "query": [
                {
                  "key": "problem",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}/configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba9035c7-6f7d-4458-9589-ae4fcba79e5e"
            }
          ]
        },
        {
          "id": "f8bece2f-31ab-4705-baa4-0f453e9e902c",
          "name": "settingssetting-idset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/{SETTING_ID}/set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a6298b5-257a-41b5-bda9-80bf575efc19"
            }
          ]
        },
        {
          "id": "705e905b-fd56-4483-a85f-eb5b2d28aadb",
          "name": "specialssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID/configuration"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9d6a4e8-f7db-49c8-8cb4-07045c6b6cd1"
            }
          ]
        },
        {
          "id": "9377481d-e8d6-4f21-a687-5ee0d28d6846",
          "name": "specialsidflag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID/retire"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{ID}/flag"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53bfeb3d-f140-4d0d-8bc2-f0073c8d577a"
            }
          ]
        }
      ]
    },
    {
      "name": "Tips",
      "item": [
        {
          "id": "bca9214e-d0ae-4851-b833-3a8eabf5516e",
          "name": "tipstip-id",
          "request": {
            "url": "http://api.foursquare.com/v2/tips/add?broadcast=%7B%7D&text=%7B%7D&url=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b9dff55-3eba-4837-8136-2a347292aeb8"
            }
          ]
        },
        {
          "id": "97fec395-6957-4cb6-a7aa-c7c0b6fc9d2b",
          "name": "tipsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/tips/search?filter=%7B%7D&limit=%7B%7D&ll=%7B%7D&offset=%7B%7D&query=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f5f03fe-6ab8-4837-93a5-c99afb27ffd9"
            }
          ]
        },
        {
          "id": "037c2798-8bc8-42c4-abff-ce7ec8ec1344",
          "name": "checkinscheckin-iddeletecomment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}/deletecomment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfa15136-796a-4f25-9eee-877d95d187bc"
            }
          ]
        },
        {
          "id": "f54b6866-c5c1-4097-b0bf-d99074d28aa1",
          "name": "tipssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/done"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd033d7a-4f8f-44fb-988a-d8c794f3b14e"
            }
          ]
        },
        {
          "id": "611be0f8-319d-4518-8ce2-89ab50f90937",
          "name": "tipstip-iddone",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/listed"
              ],
              "query": [
                {
                  "key": "group",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/done"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9497b758-c844-437b-b148-8c02aab1a8ef"
            }
          ]
        },
        {
          "id": "d5caf5af-2155-497b-be31-feb66b666db5",
          "name": "tipstip-idlisted",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/markdone"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/listed"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74bc1c25-0063-4567-bf1a-f54540f192ba"
            }
          ]
        },
        {
          "id": "5dea038c-46b4-4afa-8f98-3f69c6768a29",
          "name": "tipstip-idmarkdone",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/marktodo"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/markdone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb963ac7-d440-4fed-bbe2-3c7d8fda3302"
            }
          ]
        },
        {
          "id": "7ac32f3b-836c-4aad-9569-3499dff25f7d",
          "name": "tipstip-idmarktodo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/unmark"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/marktodo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32eb0cc1-db9d-4db7-b6bc-22395e3ac950"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "d7ff8836-0e9c-4485-848c-94bf0d0398eb",
          "name": "updatesnotifications",
          "request": {
            "url": "http://api.foursquare.com/v2/updates/marknotificationsread?highWatermark=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/updates/notifications"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebbe819d-9f53-42b0-b88a-ce374c36379d"
            }
          ]
        },
        {
          "id": "4cf97fb9-fbd3-49a1-8f66-a719945b046e",
          "name": "updatesupdate-id",
          "request": {
            "url": "http://api.foursquare.com/v2/updates/notifications?limit=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/updates/{UPDATE_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87ce9ccc-1144-4d51-a2cd-0686bd39788d"
            }
          ]
        },
        {
          "id": "497aa34c-1667-4c73-9da0-7537d75818a6",
          "name": "listslist-idupdateitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "updates/:UPDATE_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "UPDATE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/updateitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5571a12b-9061-4a90-9bd6-8b2d2e06ce19"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "fad3a64d-7a4b-4738-9ff3-8ed9f7642626",
          "name": "usersuser-id",
          "request": {
            "url": "http://api.foursquare.com/v2/users/leaderboard?neighbors=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/{USER_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef90b9f9-ff9f-47cd-94ba-43cb4e6f3e86"
            }
          ]
        },
        {
          "id": "7174bbce-af9f-4fe8-b086-24b4f88a3b01",
          "name": "usersleaderboard",
          "request": {
            "url": "http://api.foursquare.com/v2/users/requests?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/leaderboard"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "913b4ed1-2483-4b9e-ae39-6ad711c3b1bb"
            }
          ]
        },
        {
          "id": "33c76a5b-26a3-488a-b1f8-5faf14970003",
          "name": "usersrequests",
          "request": {
            "url": "http://api.foursquare.com/v2/users/search?email=%7B%7D&fbid=%7B%7D&name=%7B%7D&phone=%7B%7D&twitter=%7B%7D&twitterSource=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/users/requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4d79d04-bb86-4063-99a9-d94027ca0c08"
            }
          ]
        },
        {
          "id": "d7dae9dc-0154-4455-b610-01d61a3fcdda",
          "name": "userssearch-get",
          "request": {
            "url": "http://api.foursquare.com/v2/users/search?email=%7B%7D&fbid=%7B%7D&name=%7B%7D&phone=%7B%7D&twitter=%7B%7D&twitterSource=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "users/search (GET)"
       