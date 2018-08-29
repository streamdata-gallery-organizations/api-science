{
  "info": {
    "name": "API Science Get a Specific Monitor",
    "_postman_id": "6a0cffb1-ddb9-45bd-98db-807c161e0d84",
    "description": "Get a Specific Monitor",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitors",
      "item": [
        {
          "id": "439411bf-4719-4c8f-b5d3-edb52d5ce3b9",
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
              "id": "212ee65b-7953-4ccd-aae2-9d5e28e011ae"
            }
          ]
        },
        {
          "id": "04fa3049-6309-4cab-a9f8-2cfa4fa89352",
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
              "id": "5385e320-4387-4855-a203-9afe8c783725"
            }
          ]
        },
        {
          "id": "28a2baee-4c0a-4a4b-b013-81c716f97ed1",
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
              "id": "27f70458-0ad3-4195-8800-fde445d6dd7d"
            }
          ]
        },
        {
          "id": "60791fe2-f3d6-4860-8a30-6f5ac96dde12",
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
              "id": "aae2118d-bad7-4ca3-a632-eaf9788c4a4a"
            }
          ]
        }
      ]
    }
  ]
}