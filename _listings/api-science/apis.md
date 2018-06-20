---
name: API Science
x-slug: api-science
description: Traditional monitoring services were designed long before APIs became
  core to modern applications. API Science is designed specifically for monitoring
  APIs. Sure, we understand REST, JSON, OAuth, XML. No problem.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
x-kinRank: "10"
x-alexaRank: "0"
tags: API Science
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/apis.md
specificationVersion: "0.14"
apis:
- name: API Science Get All Contacts
  x-api-slug: api-science
  description: Get All Contacts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///contacts.json
  tags: Contacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contacts-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contacts-json-get-openapi.md
- name: API Science Create a Contact
  x-api-slug: api-science
  description: Create a Contact
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///contacts.json
  tags: Contacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contacts-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contacts-json-post-openapi.md
- name: API Science Delete a Contact
  x-api-slug: api-science
  description: Delete a Contact
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///contacts/{id}.json
  tags: Contacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contactsid-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contactsid-json-delete-openapi.md
- name: API Science Get a Specific Contact
  x-api-slug: api-science
  description: Get a Specific Contact
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///contacts/{id}.json
  tags: Contacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contactsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contactsid-json-get-openapi.md
- name: API Science Update a Contact
  x-api-slug: api-science
  description: Update a Contact
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///contacts/{id}.json
  tags: Contacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contactsid-json-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/contactsid-json-patch-openapi.md
- name: API Science Get All Monitors
  x-api-slug: api-science
  description: Marks message as read.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors
  tags: Monitors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitors-get-openapi.md
- name: API Science Create a Monitor
  x-api-slug: api-science
  description: Create a Monitor
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors
  tags: Monitors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitors-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitors-post-openapi.md
- name: API Science Apply Actions to Multiple Monitors
  x-api-slug: api-science
  description: Apply Actions to Multiple Monitors
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors
  tags: Monitors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitors-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitors-put-openapi.md
- name: API Science Get a Specific Monitor
  x-api-slug: api-science
  description: Get a Specific Monitor
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/{id}
  tags: Monitors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsid-get-openapi.md
- name: API Science Get Checks For A Monitor
  x-api-slug: api-science
  description: Get Checks For A Monitor
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/{id}/checks.json
  tags: Checks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidchecks-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidchecks-json-get-openapi.md
- name: API Science Performance Report
  x-api-slug: api-science
  description: Performance Report
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/{id}/performance
  tags: Performance
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidperformance-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidperformance-get-openapi.md
- name: API Science Show a Monitors Templates
  x-api-slug: api-science
  description: Show a Monitors Templates
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/{id}/templates
  tags: Templates
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidtemplates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidtemplates-get-openapi.md
- name: API Science Get a Template
  x-api-slug: api-science
  description: Get a Template
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/{id}/templates/{templates]
  tags: Templates
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidtemplatestemplates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidtemplatestemplates-get-openapi.md
- name: API Science Create a Template
  x-api-slug: api-science
  description: Create a Template
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/{id}/templates/{templates]
  tags: Templates
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidtemplatestemplates-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidtemplatestemplates-post-openapi.md
- name: API Science Testing your Monitor
  x-api-slug: api-science
  description: Testing your Monitor
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/{id}/test
  tags: Monitors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidtest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsidtest-get-openapi.md
- name: API Science Uptime Report
  x-api-slug: api-science
  description: Uptime Report
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/{id}/uptime.json
  tags: Uptime
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsiduptime-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsiduptime-json-get-openapi.md
- name: API Science List All Tags
  x-api-slug: api-science
  description: List All Tags
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///tags
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/tags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/tags-get-openapi.md
- name: API Science Get Contacts List
  x-api-slug: api-science
  description: Returns a list of all contacts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: |-
    https:////
        /api/{version}/contacts
  tags: Contacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/apiversioncontacts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/apiversioncontacts-get-openapi.md
- name: API Science Deleting a tag
  x-api-slug: api-science
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///inventory/tags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/inventorytags--openapi.md
- name: API Science Create Monitor
  x-api-slug: api-science
  description: Create a new monitor.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors
  tags: Monitors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitors-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitors-post-openapi.md
- name: API Science Update Monitor
  x-api-slug: api-science
  description: Update an existing monitor
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/{monitor_id}
  tags: Monitors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsmonitor-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsmonitor-id-put-openapi.md
- name: API Science Activate Monitor
  x-api-slug: api-science
  description: Activate a suspended monitor
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitors/activate/{monitor_id}
  tags: Monitors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsactivatemonitor-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorsactivatemonitor-id-put-openapi.md
- name: API Science Poll Monitor
  x-api-slug: api-science
  description: Poll a monitor.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https://///monitor/poll_now/{monitor_id}
  tags: Monitors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorpoll-nowmonitor-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/monitorpoll-nowmonitor-id-get-openapi.md
- name: API Science
  x-api-slug: api-science
  description: Traditional monitoring services were designed long before APIs became
    core to modern applications. API Science is designed specifically for monitoring
    APIs. Sure, we understand REST, JSON, OAuth, XML. No problem.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/api-science-logo.png
  humanURL: http://apiscience.com
  baseURL: https:///
  tags: API Science
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/api-science/master/_listings/api-science/openapi.md
x-common:
- type: x-base-url
  url: http://api.apiscience.com
- type: x-blog
  url: https://www.apiscience.com/blog/
- type: x-blog-rss
  url: https://www.apiscience.com/blog/feed/
- type: x-developer
  url: https://www.apiscience.com/docs/api
- type: x-pricing
  url: https://www.apiscience.com/pricing
- type: x-privacy
  url: https://www.apiscience.com/privacy
- type: x-terms-of-service
  url: https://www.apiscience.com/terms
- type: x-twitter
  url: https://twitter.com/APIScience
- type: x-website
  url: http://apiscience.com
- type: x-website
  url: http://www.apiscience.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---