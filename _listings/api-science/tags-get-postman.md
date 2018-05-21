{
  "info": {
    "name": "API Science List All Tags",
    "_postman_id": "4403a225-72c8-457d-b093-1dc125ca5e07",
    "description": "List All Tags",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "4499f6c8-961c-4a36-b578-3a07018bfa7e",
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
              "id": "f938b591-9ccc-40a7-a1e2-4502fe87e501"
            }
          ]
        },
        {
          "id": "2fb7bfae-5ee5-4d87-8b09-edbd4e6f4e26",
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
              "id": "ed2d4500-3ce0-4056-a691-0d7cfd8128d7"
            }
          ]
        },
        {
          "id": "9294bdfd-5c42-4cbe-824e-f05b6f5bfe83",
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
              "id": "9874cf63-98cf-4c6e-b328-c166818bcb31"
            }
          ]
        },
        {
          "id": "7ff4d27d-85e5-4a69-854d-2b0c1ba66365",
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
              "id": "32e9ead2-25e8-477f-aebe-84d190e831fd"
            }
          ]
        },
        {
          "id": "b85dd095-2e9d-40c4-958b-7d4fb4149d19",
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
              "id": "0749f721-d59c-441c-8c78-05dcab35fe6b"
            }
          ]
        }
      ]
    },
    {
      "name": "Monitors",
      "item": [
        {
          "id": "eccf4fd4-d907-481c-8bb2-9804659d59cb",
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
              "id": "63f6c11f-3be7-4f04-88c5-201986963b54"
            }
          ]
        },
        {
          "id": "4395fa95-7d34-4daf-8498-dc380d9ad763",
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
              "id": "6dadfee6-73f3-4283-a6ac-d7ade80c5f14"
            }
          ]
        },
        {
          "id": "6251f249-91c3-42b2-84e6-1c90aeb4d517",
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
              "id": "f001a373-569b-4d6e-b7db-2a888656047c"
            }
          ]
        },
        {
          "id": "20e1a6c1-4140-4c2e-a444-822ad9f9fc58",
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
              "id": "2c1a499e-66c3-42da-b9f4-df21927c649d"
            }
          ]
        },
        {
          "id": "630d7bcb-c72d-41f6-b107-811fb7f9657e",
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
              "id": "aec7e661-5df2-4a8b-a952-b8dbe04670a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Checks",
      "item": [
        {
          "id": "fbf88659-7d88-44b4-a903-d7f677065ea1",
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
              "id": "32a4b246-e732-4a23-984d-788e8f00a4ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "f5311b49-50a7-4f9f-8e18-fcd9a160d238",
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
              "id": "0e7c65d3-a452-447f-aefb-09caa8ae2fb7"
            }
          ]
        }
      ]
    },
    {
      "name": "Templates",
      "item": [
        {
          "id": "20c2de40-0e1c-42ec-b081-d1703bc39c89",
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
              "id": "1be9d0af-df70-45d3-85a3-9f3db2b7aa89"
            }
          ]
        },
        {
          "id": "a60ebd27-020a-408f-a40f-bc60a0fcb49f",
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
              "id": "44c98490-77cf-4997-b8a7-a7d6bb233fad"
            }
          ]
        },
        {
          "id": "3ef3e3c2-e847-4be5-b73d-474ae830508e",
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
              "id": "4f31e06b-ed65-44ad-9c28-3db97e8c8bed"
            }
          ]
        }
      ]
    },
    {
      "name": "Uptime",
      "item": [
        {
          "id": "0025d7c2-4a7e-4762-a888-8164f1138477",
          "name": "uptimeReport",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "monitors/:id/uptime.json"
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
            "description": "Uptime Report"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2eee7e07-710d-4b01-a192-33cd20df25db"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "5810b864-80f6-4efe-96b5-e581576edd34",
          "name": "listAllTags",
          "request": {
            "url": "http://example.com/api/tags?detailed=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List All Tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57b2bbe6-b4f9-4b57-b222-f9269d1ca6dd"
            }
          ]
        }
      ]
    }
  ]
}