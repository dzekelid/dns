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
  /cloudlets/api/v2/origins/currentActivations:
    get:
      summary: List Current Cloudlets Origin Activations
      description: List Current Cloudlets Origin Activations
      operationId: cloudletsapiv2originscurrentactivations
      responses:
        200:
          description: OK
      tags:
      - cloudlets
      - api
      - v2
      - origins
      - currentactivations
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