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
  /?Action=AttachStaticIp&k=1:
    get:
      summary: ' Attach Static Ip '
      description: Attaches a static IP address to a specific Amazon Lightsail instance
      operationId: attachStaticIp
      parameters:
      - in: query
        name: instanceName
        description: The instance name to which you want to attach the static IP address
        type: string
      - in: query
        name: staticIpName
        description: The name of the static IP
        type: string
      responses:
        200:
          description: OK
      tags:
      - ip addresses
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