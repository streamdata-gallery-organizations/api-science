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
  /monitors/{monitor_id}:
    put:
      summary: Update Monitor
      description: Update an existing monitor
      operationId: update-monitor
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryUnique ID of the monitor
        type: <td>string</td>
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