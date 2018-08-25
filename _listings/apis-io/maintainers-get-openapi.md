---
swagger: "2.0"
x-collection-name: APIs.io
x-complete: 0
info:
  title: APIs.io Get Maintainers
  description: Returns a list of maintainers
  version: 1.0.0
host: apis.io
basePath: api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apis:
    get:
      summary: Get APIS
      description: List all the APIs available
      operationId: getAPIs
      x-api-path-slug: apis-get
      parameters:
      - in: query
        name: fields
        description: Fields to be returned in results
        type: string
        format: string
      - in: query
        name: q
        description: keyword to search for
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - APIs
    post:
      summary: Add APIs
      description: Adds an API to APIs.io
      operationId: addAPI
      x-api-path-slug: apis-post
      parameters:
      - in: query
        name: url
        description: The URL of the APIs
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - APIs
  /search:
    get:
      summary: Search APIs
      description: Search for apis
      operationId: searchAPIs
      x-api-path-slug: search-get
      responses:
        200:
          description: OK
      tags:
      - APIs
  /maintainers:
    get:
      summary: Get Maintainers
      description: Returns a list of maintainers
      operationId: getMaintainser
      x-api-path-slug: maintainers-get
      responses:
        200:
          description: OK
      tags:
      - APIs
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