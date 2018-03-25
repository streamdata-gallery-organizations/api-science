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
  /monitors:
    get:
      summary: Get All Monitors
      description: Marks message as read
      operationId: getAllMonitors
      parameters:
      - in: header
        name: Authorization
        description: Your API key must be included in all API requests to the server
          in an Authorization HTTP header
      - in: query
        name: tags
        description: Optionally filter monitors by tags
      responses:
        200:
          description: OK
      tags:
      - monitors
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