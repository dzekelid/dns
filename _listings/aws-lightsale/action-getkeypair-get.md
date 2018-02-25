---
swagger: "2.0"
info:
  title: AWS Lightsale API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetKeyPair&k=1:
    get:
      summary: ' Get Key Pair '
      description: Returns information about a specific key pair
      operationId: getKeyPair
      parameters:
      - in: query
        name: keyPairName
        description: The name of the key pair for which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - key pairs
definitions: []
x-collection-name: AWS Lightsale
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