{
  "info": {
    "name": "API Science Activate Monitor",
    "_postman_id": "a7e71f2f-210f-4c6b-9678-05e92862eb11",
    "description": "Activate a suspended monitor",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitors",
      "item": [
        {
          "id": "fd9c4373-a527-48b6-b915-50d95772c7ae",
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
              "id": "d7a4a8c4-6d1f-4376-8fb7-61945a4ce97c"
            }
          ]
        },
        {
          "id": "2b70382a-5af1-4be9-b9e8-ee1724f2427f",
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
              "id": "b24743e0-263f-47d1-80ac-04998b8bfe60"
            }
          ]
        },
        {
          "id": "e939a85f-7c9d-4d40-9d08-696a43640bfd",
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
              "id": "fbeb2651-92e7-4106-a9c4-356bfb13b1ee"
            }
          ]
        },
        {
          "id": "348228d6-58ba-43aa-a2b8-e6583e918322",
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
              "id": "45d2b4b2-f0ec-4a17-bcd7-9218f1e56e7f"
            }
          ]
        },
        {
          "id": "045cce7a-f63d-4f8a-99f7-92d2f9d70d94",
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
              "id": "f87f9257-b048-4130-8021-4d821783d13b"
            }
          ]
        },
        {
          "id": "fccdbdb9-47ad-448c-90df-66743903af11",
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
              "id": "3ba0a67e-2ec3-4c5c-8e7c-b962b1268a59"
            }
          ]
        },
        {
          "id": "ee0897b4-7dcc-4c7f-8e8b-04914995a227",
          "name": "activate-monitor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "monitors/activate/:monitor_id"
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
            "description": "Activate a suspended monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29278cf1-8575-4afc-b42e-eb7af60723de"
            }
          ]
        }
      ]
    }
  ]
}