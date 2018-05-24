{
  "info": {
    "name": "API Science Get a Specific Contact",
    "_postman_id": "4c94e7b3-e910-4953-9586-9f01d53413ef",
    "description": "Get a Specific Contact",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "998641ff-ee42-48ad-be7d-ce869c8557da",
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
              "id": "33f7b9ea-978e-47b9-855c-43f69053a33d"
            }
          ]
        },
        {
          "id": "43c6e2e5-c358-408f-98c6-b47a480dfe06",
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
              "id": "3aa0a4e4-6168-4fae-8561-f5ba93c07e42"
            }
          ]
        },
        {
          "id": "de0f2018-5a61-45eb-a756-166efb3f484a",
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
              "id": "91fce346-123a-4144-abee-99361dc70c82"
            }
          ]
        },
        {
          "id": "4b7e48e9-c37f-4eef-9d6e-d20609a4b973",
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
              "id": "ea5df15f-20c7-4cf7-8415-6a935f174b29"
            }
          ]
        }
      ]
    }
  ]
}