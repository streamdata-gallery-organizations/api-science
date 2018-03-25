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
  /monitors/{id}/performance:
    get:
      summary: Performance Report
      description: Performance Report
      operationId: performanceReport
      parameters:
      - in: query
        name: end
        description: The end point you want to build a performance report from
      - in: path
        name: id
        description: The id for the monitor
      - in: query
        name: preset
        description: Present for commonly requested reports
      - in: query
        name: resolution
        description: The resolution is the time unit for aggregating data, with allowable
          values of hour, day, and week
      - in: query
        name: start
        description: The start point you want to build a performance report from
      responses:
        200:
          description: OK
      tags:
      - performance
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