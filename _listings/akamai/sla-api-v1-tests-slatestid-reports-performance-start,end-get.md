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
  /sla-api/v1/tests/{slaTestId}/reports/performance{?start,end}:
    get:
      summary: List Performance Reports
      description: List Performance Reports
      operationId: slaapiv1testsslatestidreportsperformancestartend
      parameters:
      - in: String
        name: end
        description: Timestamp for the end of the data window, in UTC 8601 format
        type: string
      - in: Number
        name: slaTestId
        description: Unique identifier for the test you wish to run a report on
        type: string
      - in: String
        name: start
        description: Timestamp for the start of the data window, in UTC 8601 format
        type: string
      responses:
        200:
          description: OK
      tags:
      - sla
      - api
      - v1
      - tests
      - slatest
      - reports
      - performance
      - start
      - end
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