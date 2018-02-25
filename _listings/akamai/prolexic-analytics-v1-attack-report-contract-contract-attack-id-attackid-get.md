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
  /prolexic-analytics/v1/attack-report/contract/{contract}/attack-id/{attackId}:
    get:
      summary: Get an Attack Report
      description: Get an Attack Report
      operationId: prolexicanalyticsv1attackreportcontractcontractattackidattackid
      parameters:
      - in: Number
        name: attackId
        description: Integer matching the attackId of the attack desired
        type: string
      - in: String
        name: contract
        description: Name of contract attack report belong to
        type: string
      responses:
        200:
          description: OK
      tags:
      - prolexic
      - analytics
      - v1
      - attack
      - report
      - contract
      - contract
      - attack
      - ""
      - attack
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