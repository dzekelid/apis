---
swagger: "2.0"
x-collection-name: Google API Discovery Service
x-complete: 0
info:
  title: Google API Discovery Service API Get APIs
  description: Retrieve the list of APIs supported at this endpoint.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /discovery/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apis:
    get:
      summary: Get APIs
      description: Retrieve the list of APIs supported at this endpoint.
      operationId: discovery.apis.list
      x-api-path-slug: apis-get
      parameters:
      - in: query
        name: name
        description: Only include APIs with the given name
      - in: query
        name: preferred
        description: Return only the preferred version of an API
      responses:
        200:
          description: OK
      tags:
      - API
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