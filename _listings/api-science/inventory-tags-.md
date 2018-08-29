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
  /inventory/tags:
    "":
      summary: Deleting a tag
      description: ""
      operationId: deleting-a-tag
      parameters:
      - in: body
        name: color
        description: The color of the tag in hexcode
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: name
        description: Name of the tag
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: token
        description: Your API token
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - tags
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