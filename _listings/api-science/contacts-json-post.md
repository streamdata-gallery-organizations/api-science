---
swagger: "2.0"
info:
  title: API Science
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts.json:
    post:
      summary: Create a Contact
      description: Create a Contact
      operationId: createContact
      parameters:
      - in: formData
        name: label
        description: User-defined label for this contact
      - in: formData
        name: type
        description: 'Type of contact, options are: email, url, pagerduty'
      - in: formData
        name: value
        description: 'Contents of value vary based on the type of contact being created:
          an email address, a URL or your PagerDuty API key'
      responses:
        200:
          description: OK
      tags:
      - contacts
definitions: []
x-collection-name: API Science
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---