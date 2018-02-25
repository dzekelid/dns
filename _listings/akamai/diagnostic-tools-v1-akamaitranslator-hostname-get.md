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
  /diagnostic-tools/v1/akamaitranslator{?hostname}:
    get:
      summary: Translate Hostname
      description: Translate Hostname
      operationId: diagnostictoolsv1akamaitranslatorhostname
      parameters:
      - in: String
        name: hostname
        description: Hostname for which to retrieve ARL information
        type: string
      responses:
        200:
          description: OK
      tags:
      - diagnostic
      - tools
      - v1
      - akamaitranslator
      - hostname
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