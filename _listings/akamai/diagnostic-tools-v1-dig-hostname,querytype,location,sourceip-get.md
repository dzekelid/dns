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
  /diagnostic-tools/v1/dig{?hostname,queryType,location,sourceIp}:
    get:
      summary: Run dig
      description: Run dig
      operationId: diagnostictoolsv1dighostnamequerytypelocationsourceip
      parameters:
      - in: String
        name: hostname
        description: the domain name you want to get information about
        type: string
      - in: String
        name: location
        description: Location of Akamai server from which you want to run dig
        type: string
      - in: Enumeration
        name: queryType
        description: 'query type for the dig; valid types are:'
        type: string
      - in: String
        name: sourceIp
        description: CDN server IP to run DIG from
        type: string
      responses:
        200:
          description: OK
      tags:
      - diagnostic
      - tools
      - v1
      - dig
      - hostname
      - querytype
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