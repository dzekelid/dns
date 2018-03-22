---
swagger: "2.0"
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CheckDNSAvailability:
    get:
      summary: ' Check D N S Availability '
      description: Checks if the specified CNAME is available
      operationId: checkDNSAvailability
      parameters:
      - in: query
        name: CNAMEPrefix
        description: The prefix used when this CNAME is reserved
        type: string
      responses:
        200:
          description: OK
      tags:
      - dns
definitions: []
x-collection-name: AWS Elastic Beanstalk
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