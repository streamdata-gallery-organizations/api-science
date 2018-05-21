{
  "info": {
    "name": "API Science Get All Monitors",
    "_postman_id": "69a5689a-d3fc-43d3-8669-bf033dc722bd",
    "description": "Marks message as read.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitors",
      "item": [
        {
          "id": "a81c2452-8671-43d8-9143-7619ca22bcc2",
          "name": "getAllMonitors",
          "request": {
            "url": "http://example.com/api/monitors?tags=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Your API key must be included in all API requests to the server in an Authorization HTTP header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Marks message as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8b96b8d-746b-493e-a41d-208108d3ee47"
            }
          ]
        }
      ]
    }
  ]
}