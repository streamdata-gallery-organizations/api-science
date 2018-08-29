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
  ? |2-

        /api/{version}/contacts
  : get:
      summary: Get Contacts List
      description: |2-

            Returns a list of all contacts
      operationId: get-contacts-list
      parameters:
      - in: query
        name: limit
        description: Limits the number of returned contacts to the specified quantity
        type: <td>integer</td>
      - in: query
        name: offset
        description: Offset for listing
        type: <td>integer</td>
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