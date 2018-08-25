---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 1
info:
  title: PagerDuty
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api_reference:
    get:
      summary: REST API Reference
      description: REST API Reference.
      operationId: rest-api-reference
      x-api-path-slug: api-reference-get
      responses:
        200:
          description: OK
      tags:
      - APIs
---