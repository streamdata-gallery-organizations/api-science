{
  "info": {
    "name": "API Science Uptime Report",
    "_postman_id": "eb46b192-a390-42d6-a14c-07f16beb5f06",
    "description": "Uptime Report",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "06412be7-8129-4f6d-a851-11cb2fa66dc6",
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
              "id": "6e38a221-8b43-4e81-b36c-b73a7af4bd5f"
            }
          ]
        },
        {
          "id": "e3e3a2c6-9fed-4963-8dce-100ce2378f1b",
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
              "id": "d5e8ff2c-0edd-48ed-b899-4f5b1edd94d7"
            }
          ]
        },
        {
          "id": "1136a5f7-ba11-40c5-bfa9-fafe21cd49a9",
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
              "id": "a69712e2-fb7d-4bf4-b8ab-9c10ddfa671f"
            }
          ]
        },
        {
          "id": "70d6b89f-6d1b-4675-af15-a888ba611bd8",
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
              "id": "90a76645-1e6c-47ff-8d26-761ba37c65dc"
            }
          ]
        },
        {
          "id": "23f73190-57a8-440a-af89-a74632a69638",
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
              "id": "0797ea65-2e65-4dd3-9a25-5a00a5e952cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Monitors",
      "item": [
        {
          "id": "4fd45feb-d8f9-45dc-903b-6278b1c6ba8a",
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
              "id": "0347c6f2-b31e-4561-bddc-cbcbec5895d5"
            }
          ]
        },
        {
          "id": "0b1c0dc9-8693-4b56-9865-f4ad5f5b4465",
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
              "id": "af5dc6af-6b41-4f70-a5f7-8e7f2fe886ba"
            }
          ]
        },
        {
          "id": "64c429e8-436f-483b-a2d8-cccb21a5f8b0",
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
              "id": "873a30b2-1164-4558-b5f2-9fd9b5fa08dc"
            }
          ]
        },
        {
          "id": "9100d3cd-721a-445d-8532-9d6e5ca3f961",
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
              "id": "1d51aee3-3f09-4bc4-9c0c-63a0f7d526c9"
            }
          ]
        },
        {
          "id": "b7e22788-46b4-4513-982f-072498a0580f",
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
              "id": "c0e5cba8-fc4b-47e1-82fc-6044e5eba58d"
            }
          ]
        }
      ]
    },
    {
      "name": "Checks",
      "item": [
        {
          "id": "b330afe7-decd-4a24-89b3-d3c0239ff440",
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
              "id": "85cb7055-c9b2-4871-b0f0-c5b84c67860a"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "bef96c31-8773-447b-9a6f-e73b201a9671",
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
              "id": "d29b292a-e21c-4316-a007-a0f81864291a"
            }
          ]
        }
      ]
    },
    {
      "name": "Templates",
      "item": [
        {
          "id": "17181fb2-3f6f-4cba-a18e-bad1b355193d",
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
              "id": "2f43ebb9-698e-44d0-8186-c23c372adb98"
            }
          ]
        },
        {
          "id": "212d5bd8-594b-4a29-a309-459e3426d8b7",
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
              "id": "60f3be77-78ee-4659-978f-6dccb0c62320"
            }
          ]
        },
        {
          "id": "f0ce78d9-3cda-40be-a4a8-bb40c162dff5",
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
              "id": "2e053c29-f2a1-47fb-9bbe-6d73c75fe717"
            }
          ]
        }
      ]
    },
    {
      "name": "Uptime",
      "item": [
        {
          "id": "46492d0a-a9f7-4a35-a8f9-e6191289739e",
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
              "id": "4b997b49-13c8-4a98-887c-c38a7b70faba"
            }
          ]
        }
      ]
    }
  ]
}