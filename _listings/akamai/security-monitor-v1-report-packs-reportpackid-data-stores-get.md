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
  /security-monitor/v1/report-packs/{reportPackId}/data-stores:
    get:
      summary: List Data Stores
      description: List Data Stores
      operationId: securitymonitorv1reportpacksreportpackiddatastores
      parameters:
      - in: Number
        name: reportPackId
        description: Report pack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - security
      - monitor
      - v1
      - report
      - packs
      - reportpack
      - data
      - stores
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