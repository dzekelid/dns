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
  /?Action=UpdateDomainEntry&k=1:
    get:
      summary: ' Update Domain Entry '
      description: Updates a domain recordset after it is created
      operationId: updateDomainEntry
      parameters:
      - in: query
        name: domainEntry
        description: An array of key-value pairs containing information about the
          domain entry
        type: string
      - in: query
        name: domainName
        description: The name of the domain recordset to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - domains
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