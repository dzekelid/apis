---
swagger: "2.0"
x-collection-name: Google API Discovery Service
x-complete: 1
info:
  title: APIs Discovery Service
  description: provides-information-about-other-google-apis-such-as-what-apis-are-available-the-resource-and-method-details-for-each-api-
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
---