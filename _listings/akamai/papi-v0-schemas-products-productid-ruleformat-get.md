---
swagger: "2.0"
info:
  title: Akamai Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /papi/v0/schemas/products/{productId}/{ruleFormat}:
    get:
      summary: Get a Rule Format&#8217;s JSON Schema
      description: Get a Rule Format&#8217;s JSON Schema
      operationId: papiv0schemasproductsproductidruleformat
      parameters:
      - in: String
        name: productId
        description: Unique identifier for the product
        type: string
      - in: String
        name: ruleFormat
        description: Name of the rule format, either one frozen to a specific date,
          or representing the latest set of behaviors and criteria
        type: string
      responses:
        200:
          description: OK
      tags:
      - papi
      - v0
      - schemas
      - products
      - product
      - ruleformat
definitions: []
x-collection-name: Akamai
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