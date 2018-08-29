{
  "info": {
    "name": "API Science Show a Monitors Templates",
    "_postman_id": "bae4ff31-c3d0-4392-97b3-f0a45e247cbd",
    "description": "Show a Monitors Templates",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "ee344bfd-930a-49a1-91b6-10ecd4a66f4f",
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
              "id": "3a1bcda3-a990-4b9d-bd32-2e48a629a6ba"
            }
          ]
        },
        {
          "id": "4c611145-aaac-413f-aa6c-1bf53c0d202a",
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
              "id": "4a9043ba-9df3-4cf9-9299-54c45d6f6864"
            }
          ]
        },
        {
          "id": "377991ed-c283-4914-b0ce-a6d6bc8dd5cc",
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
              "id": "dde21f78-846e-438f-a144-eb014eeb62cd"
            }
          ]
        },
        {
          "id": "3dce72fa-9232-4901-ad18-7f8054ec1801",
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
              "id": "d7ef1bae-e1ca-4ad5-8337-130b9e0a86d8"
            }
          ]
        },
        {
          "id": "cdd2b9d4-6777-4941-98ba-c399d2cf607d",
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
              "id": "11b0af48-a916-4ea2-ab07-7534f618a94c"
            }
          ]
        }
      ]
    },
    {
      "name": "Monitors",
      "item": [
        {
          "id": "d3453dc0-21cb-4a08-8826-e63dd9eec9c3",
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
              "id": "2d2436f7-bbf1-4d37-8732-7d24640e849c"
            }
          ]
        },
        {
          "id": "ddcf612b-2ff0-4952-a376-5af42a3704a7",
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
              "id": "11227291-d22f-4677-82f9-cc364a2ccc27"
            }
          ]
        },
        {
          "id": "f996b045-b451-4bf0-ac5f-d4f015581949",
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
              "id": "35813159-5bff-4d83-b2f2-1126e1e80e1b"
            }
          ]
        },
        {
          "id": "474a0f9e-191f-4554-b473-03dee56c9b97",
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
              "id": "19977c3f-70ac-4110-816a-4d70c369e403"
            }
          ]
        }
      ]
    },
    {
      "name": "Checks",
      "item": [
        {
          "id": "53848b4b-967f-4077-b30f-f58edef68480",
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
              "id": "434d608c-6075-40b8-b6d8-a6db94702eff"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "bc10a45a-23d7-442a-aa86-b55e96795fda",
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
              "id": "74eb81d0-8b22-41fc-b0f8-9b4939642fe2"
            }
          ]
        }
      ]
    },
    {
      "name": "Templates",
      "item": [
        {
          "id": "1690b5d3-f33b-414a-8bd7-f50cf20ac2b4",
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
              "id": "8ce47ee9-0aad-460b-b46e-08e46488b46a"
            }
          ]
        }
      ]
    }
  ]
}