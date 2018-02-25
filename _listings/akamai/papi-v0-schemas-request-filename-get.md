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
  /papi/v0/schemas/request/{filename}:
    get:
      summary: Get a Request&#8217;s JSON Schema
      description: Get a Request&#8217;s JSON Schema
      operationId: papiv0schemasrequestfilename
      parameters:
      - in: String
        name: filename
        description: Schema&#8217;s filename
        type: string
      responses:
        200:
          description: OK
      tags:
      - papi
      - v0
      - schemas
      - request
      - filename
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