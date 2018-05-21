{
  "info": {
    "name": "API Science Create a Template",
    "_postman_id": "67ca630a-48d6-4d6d-8e8d-608c53f34f9e",
    "description": "Create a Template",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "e0d37139-cc13-4168-afe6-394ed37a1474",
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
              "id": "d79ebdfe-9e50-47df-84d4-4c457c704948"
            }
          ]
        },
        {
          "id": "20a2229c-780f-4ac0-abcb-8e14ad83d2d1",
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
              "id": "e04a4703-53d8-4536-8fe2-7a2f33ef956d"
            }
          ]
        },
        {
          "id": "bf009ed4-67ca-442c-b587-7fcf38aa00f2",
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
              "id": "27d35368-bea1-4595-9603-22b7f9cd33e4"
            }
          ]
        },
        {
          "id": "4a538b29-7c69-4084-9c59-2d304818f8c4",
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
              "id": "0ee5e1eb-13ca-4527-b71e-a7eac9368d85"
            }
          ]
        },
        {
          "id": "81235d65-0c17-42f5-92a4-c1140a8b6319",
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
              "id": "9c050584-9eca-4b33-9700-9130aed776ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Monitors",
      "item": [
        {
          "id": "c12211dd-5e51-40cc-9f16-a1f96edbaad2",
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
              "id": "42c699f7-a0a6-43ae-9742-b6f3f5f6f3d8"
            }
          ]
        },
        {
          "id": "c6754ed3-95d1-4dcc-98c8-8c7173a99949",
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
              "id": "979c1e8e-6dbe-4349-9e74-dbc41de159d8"
            }
          ]
        },
        {
          "id": "6b1f3f51-1c33-4713-bea4-aff46c7342ea",
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
              "id": "3d9c105e-d30e-4ec5-b162-9846b3546289"
            }
          ]
        },
        {
          "id": "a267705c-d253-4336-88b5-cc309da9bb00",
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
              "id": "2fa94066-b084-4ee4-b3d7-9ea83acd4316"
            }
          ]
        }
      ]
    },
    {
      "name": "Checks",
      "item": [
        {
          "id": "3bfe88f4-3e59-4396-828d-3a718feb6ae5",
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
              "id": "e676aa10-612d-425b-a78d-72886fc7d77a"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "0d8b8ef2-890e-4481-976d-0132fdd7eeeb",
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
              "id": "c109e3d0-5728-45ff-bdae-8fdca333efa5"
            }
          ]
        }
      ]
    },
    {
      "name": "Templates",
      "item": [
        {
          "id": "117e5635-0efc-4d2f-b824-8ebbfd4e911c",
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
              "id": "550db061-e605-4647-9165-40970e956023"
            }
          ]
        },
        {
          "id": "86cda071-1cce-496d-9222-0e854a8e2e6a",
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
              "id": "a861c23a-79ce-49e0-86df-967049ef62c3"
            }
          ]
        },
        {
          "id": "a981527a-45ff-4464-971b-e20dc1bf9e6e",
          "name": "createTemplate",
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
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "Raw body to be send with the request"
                },
                {
                  "key": "followRedirects",
                  "value": "{}",
                  "disabled": false,
                  "description": "True if this call should automatically follow HTTP redirects (default is False)"
                },
                {
                  "key": "headers",
                  "value": "{}",
                  "disabled": false,
                  "description": "An array of key/value pairs to send as URL parameters"
                },
                {
                  "key": "method",
                  "value": "{}",
                  "disabled": false,
                  "description": "The HTTP action to access the given URL"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the template"
                },
                {
                  "key": "preProcessScript",
                  "value": "{}",
                  "disabled": false,
                  "description": "JavaScript to be executed prior to running this template"
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The URL to be accessed"
                },
                {
                  "key": "validations",
                  "value": "{}",
                  "disabled": false,
                  "description": "An array of validation objects to be run on the results of this template"
                }
              ]
            },
            "description": "Create a Template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e0da0ca-cb6a-4650-bfd5-7edc6fc7e9c9"
            }
          ]
        }
      ]
    }
  ]
}