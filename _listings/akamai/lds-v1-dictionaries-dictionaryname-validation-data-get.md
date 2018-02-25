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
  /lds/v1/dictionaries/{dictionaryName}/validation/data:
    get:
      summary: Get Validation Context
      description: Get Validation Context
      operationId: ldsv1dictionariesdictionarynamevalidationdata
      parameters:
      - in: Enumeration
        name: dictionaryName
        description: Dictionary name value
        type: string
      responses:
        200:
          description: OK
      tags:
      - lds
      - v1
      - dictionaries
      - dictionaryname
      - valation
      - data
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