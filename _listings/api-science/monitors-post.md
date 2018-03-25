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
    post:
      summary: Create a Monitor
      description: Create a Monitor
      operationId: createMonitor
      parameters:
      - in: formData
        name: active
        description: This flag determines whether the monitor is either running or
          paused
      - in: formData
        name: frequency
        description: The frequency that you want this monitor to be run at
      - in: formData
        name: name
        description: The name of the monitor
      - in: formData
        name: templates
        description: An array of template objects to be created
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