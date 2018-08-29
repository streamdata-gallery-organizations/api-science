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
  /monitors/{id}/checks.json:
    get:
      summary: Get Checks For A Monitor
      description: Get Checks For A Monitor
      operationId: getChecksForAMonitor
      parameters:
      - in: query
        name: count
        description: The number of checks to return
      - in: path
        name: id
        description: id for the monitors
      - in: query
        name: start
        description: The start number represents which ID is the maximum check that
          could be found
      responses:
        200:
          description: OK
      tags:
      - checks
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