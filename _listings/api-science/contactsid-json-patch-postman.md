{
  "info": {
    "name": "API Science Update a Contact",
    "_postman_id": "caaa2f78-6247-4c43-a6d7-330d1966e190",
    "description": "Update a Contact",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "4fe97cca-6e96-4187-aeab-0f11f8146bcb",
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
              "id": "657c7276-4615-444d-9d36-3523524fc182"
            }
          ]
        },
        {
          "id": "6ee296c9-02e7-4c97-b87b-968ce0f6f4fa",
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
              "id": "9a43750d-acb7-4411-980e-fcb1868a7cb2"
            }
          ]
        },
        {
          "id": "531e1711-513f-4233-9175-7a0e90f7e006",
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
              "id": "891617de-759a-4db4-85a0-197254742cb3"
            }
          ]
        },
        {
          "id": "52f4a570-8bb3-4777-8681-7878bea2aaa7",
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
              "id": "6cb07869-78c4-416b-8e9d-ee01b6790c9f"
            }
          ]
        },
        {
          "id": "d129dc5d-6590-4681-8c86-539a330682e1",
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
              "id": "0dca9e49-ad0d-427c-9582-2f0a7af40e5a"
            }
          ]
        }
      ]
    }
  ]
}