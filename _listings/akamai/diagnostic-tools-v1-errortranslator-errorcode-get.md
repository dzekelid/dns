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
  /diagnostic-tools/v1/errortranslator{?errorCode}:
    get:
      summary: Translate Error Code
      description: Translate Error Code
      operationId: diagnostictoolsv1errortranslatorerrorcode
      parameters:
      - in: String
        name: errorCode
        description: Error code or reference number you want to translate, which typically
          appears on an error page
        type: string
      responses:
        200:
          description: OK
      tags:
      - diagnostic
      - tools
      - v1
      - errortranslator
      - errorcode
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