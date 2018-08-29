{
  "info": {
    "name": "API Science Create Monitor",
    "_postman_id": "b3135ca3-055a-4aec-80dd-011cbf149fd1",
    "description": "Create a new monitor.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitors",
      "item": [
        {
          "id": "efc133e7-4c6a-43d2-9b42-f3a6d0bdcb16",
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
              "id": "7bf918a2-33fb-486c-8d67-de58d583ad0f"
            }
          ]
        },
        {
          "id": "fe327e35-b90d-4996-b57c-a8f2d56bac3e",
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
              "id": "77e2df3c-31ec-4681-b9a5-2763f0b40ee8"
            }
          ]
        },
        {
          "id": "4d9e7bf6-2788-4876-800a-a2ea597f38df",
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
              "id": "03a999bf-6ff6-4794-a0eb-d35483d41cd0"
            }
          ]
        },
        {
          "id": "6ab3a95e-9764-425c-98ad-8847743c3a05",
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
              "id": "16ec2393-a536-4f25-b9c8-60205cccc977"
            }
          ]
        },
        {
          "id": "d5f01185-a4a2-4f50-ba83-49fa73021ac2",
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
              "id": "17e43d29-5a34-4f03-a216-e522ffc6878d"
            }
          ]
        }
      ]
    }
  ]
}