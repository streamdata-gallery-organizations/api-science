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
  /monitors/{id}/templates/{templates]:
    post:
      summary: Create a Template
      description: Create a Template
      operationId: createTemplate
      parameters:
      - in: formData
        name: body
        description: Raw body to be send with the request
      - in: formData
        name: followRedirects
        description: True if this call should automatically follow HTTP redirects
          (default is False)
      - in: formData
        name: headers
        description: An array of key/value pairs to send as URL parameters
      - in: formData
        name: method
        description: The HTTP action to access the given URL
      - in: formData
        name: name
        description: The name of the template
      - in: formData
        name: preProcessScript
        description: JavaScript to be executed prior to running this template
      - in: formData
        name: url
        description: The URL to be accessed
      - in: formData
        name: validations
        description: An array of validation objects to be run on the results of this
          template
      responses:
        200:
          description: OK
      tags:
      - templates
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