{
  "info": {
    "name": "API Science Testing your Monitor",
    "_postman_id": "52ae4474-08b2-4ab7-855b-2faaa3b59cd6",
    "description": "Testing your Monitor",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitors",
      "item": [
        {
          "id": "ae01dda5-48a9-4acb-8652-90562ba4e68e",
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
              "id": "8c3abe70-5ea5-4aee-ad1b-308d525b2467"
            }
          ]
        },
        {
          "id": "2a6044ae-9134-4b53-8816-a26c914e9903",
          "name": "applyActionsToMultipleMonitors",
          "request": {
            "url": "http://example.com/api/monitors?tags=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Apply Actions to Multiple Monitors"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4639c834-7ab9-4879-a62c-235efc514654"
            }
          ]
        },
        {
          "id": "f60c6c6e-51aa-4091-8e0b-ea82ad2f05e1",
          "name": "createMonitor",
          "request": {
            "url": "http://example.com/api/monitors",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "This flag determines whether the monitor is either running or paused"
                },
                {
                  "key": "frequency",
                  "value": "{}",
                  "disabled": false,
                  "description": "The frequency that you want this monitor to be run at"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the monitor"
                },
                {
                  "key": "templates",
                  "value": "{}",
                  "disabled": false,
                  "description": "An array of template objects to be created"
                }
              ]
            },
            "description": "Create a Monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54e6940e-dca4-4c86-9b5d-bdc9f9f22ceb"
            }
          ]
        },
        {
          "id": "d6918b42-f912-4122-952a-42b1be9c02e2",
          "name": "getMonitor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "monitors/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a Specific Monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "344b7573-2bae-4921-9755-f5e1933c6054"
            }
          ]
        },
        {
          "id": "57606e8e-cadd-4932-af77-67e466d10062",
          "name": "testMonitor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "monitors/:id/test"
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
            "description": "Testing your Monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64b7c1f3-85e8-429c-a67c-6d7515a258eb"
            }
          ]
        }
      ]
    }
  ]
}