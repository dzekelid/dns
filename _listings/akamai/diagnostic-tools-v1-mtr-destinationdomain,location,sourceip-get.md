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
  /diagnostic-tools/v1/mtr{?destinationDomain,location,sourceIp}:
    get:
      summary: Run mtr
      description: Run mtr
      operationId: diagnostictoolsv1mtrdestinationdomainlocationsourceip
      parameters:
      - in: String
        name: destinationDomain
        description: The domain name you want to get information about
        type: string
      - in: String
        name: location
        description: Location of Akamai Server you want to run dig from
        type: string
      - in: String
        name: sourceIp
        description: CDN server IP to run MTR from
        type: string
      responses:
        200:
          description: OK
      tags:
      - diagnostic
      - tools
      - v1
      - mtr
      - destinationdomain
      - location
      - sourceip
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