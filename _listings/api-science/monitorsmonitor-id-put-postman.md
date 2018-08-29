{
  "info": {
    "name": "API Science Update Monitor",
    "_postman_id": "8f857734-43a6-45a4-9e90-a88a6f928fb0",
    "description": "Update an existing monitor",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitors",
      "item": [
        {
          "id": "734a81b5-795c-48d6-b349-72eccbf19928",
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
              "id": "bd8b565a-009f-4ae0-84bf-6fbc7f999491"
            }
          ]
        },
        {
          "id": "c93d1866-c53b-44b6-ac9f-a50615f27283",
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
              "id": "c83a8983-0d30-428a-b1a0-b18d3939df91"
            }
          ]
        },
        {
          "id": "80da3e30-05ee-401f-a780-610d14b3011e",
          "name": "create-monitor",
          "request": {
            "url": "http://example.com/api/monitors",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new monitor."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fceb9da-9406-4fca-9e32-b2edec180990"
            }
          ]
        },
        {
          "id": "9df12daa-7134-4b58-bf62-980f21076eda",
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
              "id": "2e73ad72-be01-4d5b-af3b-6f42a60e269f"
            }
          ]
        },
        {
          "id": "205585f8-ede1-4c91-b4cf-974e2e7261fb",
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
              "id": "75e5f3bd-c1d9-41ee-b612-01489a3c5df3"
            }
          ]
        },
        {
          "id": "3ddcde2f-e7e2-4630-acdf-68b2dbb41921",
          "name": "update-monitor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "monitors/:monitor_id"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c86e9fc9-a3d9-4da8-8f28-d89c61dcd96f"
            }
          ]
        }
      ]
    }
  ]
}