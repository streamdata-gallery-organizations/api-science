{
  "info": {
    "name": "API Science Get a Template",
    "_postman_id": "44a2cb74-2148-49af-8d3f-bcb03cb0f651",
    "description": "Get a Template",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "9fd69032-c6dc-4d33-9180-4b4f0460eddf",
          "name": "getAllContacts",
          "request": {
            "url": "http://example.com/api/contacts.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get All Contacts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "438d7ef3-bdb7-4bac-9a1d-eddc42afb559"
            }
          ]
        },
        {
          "id": "b3003b5b-88d8-46e0-bbba-3484feb031b5",
          "name": "createContact",
          "request": {
            "url": "http://example.com/api/contacts.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "label",
                  "value": "{}",
                  "disabled": false,
                  "description": "User-defined label for this contact"
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": "Type of contact, options are: email, url, pagerduty"
                },
                {
                  "key": "value",
                  "value": "{}",
                  "disabled": false,
                  "description": "Contents of value vary based on the type of contact being created: an email address, a URL or your PagerDuty API key"
                }
              ]
            },
            "description": "Create a Contact"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "936512a1-0568-469b-a237-f12726e5404a"
            }
          ]
        },
        {
          "id": "9df5ae57-aa5e-4c14-acab-3b816deeb89b",
          "name": "getContact",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "contacts/:id.json"
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
            "description": "Get a Specific Contact"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "025a4669-7cee-44b1-b27e-f8dbbfb0cdd5"
            }
          ]
        },
        {
          "id": "6cd46985-b3d9-458b-84d9-0b08f7800bb8",
          "name": "deleteContact",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "contacts/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a Contact"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab86fd40-731b-435a-9b98-039d0349c586"
            }
          ]
        },
        {
          "id": "530bd8db-fe9a-4413-becd-7be8d7d7890b",
          "name": "updateContact",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "contacts/:id.json"
              ],
              "query": [
                {
                  "key": "value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "label",
                  "value": "{}",
                  "disabled": false,
                  "description": "User-defined label for this contact"
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": "Type of contact, options are: email, url, pagerduty"
                }
              ]
            },
            "description": "Update a Contact"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a21b827b-b233-431c-b80e-e838635467f0"
            }
          ]
        }
      ]
    },
    {
      "name": "Monitors",
      "item": [
        {
          "id": "02050699-c65b-4f6d-9f70-ec1c8d7379df",
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
              "id": "b75ebf28-c7c2-48db-9e16-6f5f6fececfb"
            }
          ]
        },
        {
          "id": "250006ec-2d79-40c0-994a-4422d87bdd45",
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
              "id": "74af99e4-da54-4c79-a67c-83fe5d161d0a"
            }
          ]
        },
        {
          "id": "2fac0a2f-0cda-4375-a091-4fd60b7ebce2",
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
              "id": "2df6fcc7-ddb0-4248-99b5-810ea3284b54"
            }
          ]
        },
        {
          "id": "2c7bf1f6-ce2d-4c28-9825-370fd2b776c5",
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
              "id": "15f0f3f0-0d01-4cf4-9cd1-39868ea4f204"
            }
          ]
        }
      ]
    },
    {
      "name": "Checks",
      "item": [
        {
          "id": "db4ea0b4-4f05-4110-be20-d5991511b680",
          "name": "getChecksForAMonitor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "monitors/:id/checks.json"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Get Checks For A Monitor"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88390db1-2d48-4d6f-915a-96b941e33eec"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "0e0bfe3c-676b-4ac7-9e8a-57ffc47e28b3",
          "name": "performanceReport",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "monitors/:id/performance"
              ],
              "query": [
                {
                  "key": "end",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "preset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "resolution",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Performance Report"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e62c891c-0da5-4390-b337-c82a64ddf26f"
            }
          ]
        }
      ]
    },
    {
      "name": "Templates",
      "item": [
        {
          "id": "dd90ba55-befa-4e72-985c-62461e3ccfdc",
          "name": "showMonitorsTemplates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "monitors/:id/templates"
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
            "description": "Show a Monitors Templates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6da8cce1-a98c-4b16-bb01-9071e0524075"
            }
          ]
        },
        {
          "id": "09e70098-babb-41a5-9ec1-3fde736e6366",
          "name": "getTemplate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "monitors/:id/templates/{templates]"
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
            "description": "Get a Template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c995d22-871c-4ec4-8e36-2c8523401ff6"
            }
          ]
        }
      ]
    }
  ]
}