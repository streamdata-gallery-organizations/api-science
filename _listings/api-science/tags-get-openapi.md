---
swagger: "2.0"
x-collection-name: API Science
x-complete: 0
info:
  title: API Science List All Tags
  version: 1.0.0
  description: List All Tags
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts.json:
    get:
      summary: Get All Contacts
      description: Get All Contacts
      operationId: getAllContacts
      x-api-path-slug: contactsjson-get
      responses:
        200:
          description: OK
      tags:
      - Contacts
    post:
      summary: Create a Contact
      description: Create a Contact
      operationId: createContact
      x-api-path-slug: contactsjson-post
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
      - Contacts
  /contacts/{id}.json:
    delete:
      summary: Delete a Contact
      description: Delete a Contact
      operationId: deleteContact
      x-api-path-slug: contactsidjson-delete
      parameters:
      - in: path
        name: id
        description: The id for the contact
      responses:
        200:
          description: OK
      tags:
      - Contacts
    get:
      summary: Get a Specific Contact
      description: Get a Specific Contact
      operationId: getContact
      x-api-path-slug: contactsidjson-get
      parameters:
      - in: path
        name: id
        description: The ID of the contact to retrieve
      responses:
        200:
          description: OK
      tags:
      - Contacts
    patch:
      summary: Update a Contact
      description: Update a Contact
      operationId: updateContact
      x-api-path-slug: contactsidjson-patch
      parameters:
      - in: path
        name: id
        description: ID for the contact
      - in: formData
        name: label
        description: User-defined label for this contact
      - in: formData
        name: type
        description: 'Type of contact, options are: email, url, pagerduty'
      - in: query
        name: value
        description: 'Contents of value vary based on the type of contact being created:
          an email address, a URL or your PagerDuty API key'
      responses:
        200:
          description: OK
      tags:
      - Contacts
  /monitors:
    get:
      summary: Get All Monitors
      description: Marks message as read.
      operationId: getAllMonitors
      x-api-path-slug: monitors-get
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
      - Monitors
    post:
      summary: Create a Monitor
      description: Create a Monitor
      operationId: createMonitor
      x-api-path-slug: monitors-post
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
      - Monitors
    put:
      summary: Apply Actions to Multiple Monitors
      description: Apply Actions to Multiple Monitors
      operationId: applyActionsToMultipleMonitors
      x-api-path-slug: monitors-put
      parameters:
      - in: path
        name: tags
        description: Optionally filter monitors by tags
      responses:
        200:
          description: OK
      tags:
      - Monitors
  /monitors/{id}:
    get:
      summary: Get a Specific Monitor
      description: Get a Specific Monitor
      operationId: getMonitor
      x-api-path-slug: monitorsid-get
      parameters:
      - in: path
        name: id
        description: The ID of the monitor to retrieve
      responses:
        200:
          description: OK
      tags:
      - Monitors
  /monitors/{id}/checks.json:
    get:
      summary: Get Checks For A Monitor
      description: Get Checks For A Monitor
      operationId: getChecksForAMonitor
      x-api-path-slug: monitorsidchecksjson-get
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
      - Checks
  /monitors/{id}/performance:
    get:
      summary: Performance Report
      description: Performance Report
      operationId: performanceReport
      x-api-path-slug: monitorsidperformance-get
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
      - Performance
  /monitors/{id}/templates:
    get:
      summary: Show a Monitors Templates
      description: Show a Monitors Templates
      operationId: showMonitorsTemplates
      x-api-path-slug: monitorsidtemplates-get
      parameters:
      - in: path
        name: id
        description: The id for the monitor
      responses:
        200:
          description: OK
      tags:
      - Templates
  /monitors/{id}/templates/{templates]:
    get:
      summary: Get a Template
      description: Get a Template
      operationId: getTemplate
      x-api-path-slug: monitorsidtemplatestemplates-get
      responses:
        200:
          description: OK
      tags:
      - Templates
    post:
      summary: Create a Template
      description: Create a Template
      operationId: createTemplate
      x-api-path-slug: monitorsidtemplatestemplates-post
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
      - Templates
  /monitors/{id}/test:
    get:
      summary: Testing your Monitor
      description: Testing your Monitor
      operationId: testMonitor
      x-api-path-slug: monitorsidtest-get
      responses:
        200:
          description: OK
      tags:
      - Monitors
  /monitors/{id}/uptime.json:
    get:
      summary: Uptime Report
      description: Uptime Report
      operationId: uptimeReport
      x-api-path-slug: monitorsiduptimejson-get
      parameters:
      - in: query
        name: end
        description: The end point you want to build a performance report from
      - in: path
        name: id
        description: Id for the monitor
      - in: query
        name: preset
        description: Present for commonly requested reports
      - in: query
        name: resolution
        description: The resolution is the time unit for aggregating data, with allowable
          values of hourly, daily, and weekly
      - in: query
        name: start
        description: The start point you want to build a performance report from
      responses:
        200:
          description: OK
      tags:
      - Uptime
  /tags:
    get:
      summary: List All Tags
      description: List All Tags
      operationId: listAllTags
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: detailed
        description: Detailed List All Tags
      responses:
        200:
          description: OK
      tags:
      - Tags
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