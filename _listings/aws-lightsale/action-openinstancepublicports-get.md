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
  /?Action=OpenInstancePublicPorts&k=1:
    get:
      summary: ' Open Instance Public Ports '
      description: Adds public ports to an Amazon Lightsail instance
      operationId: openInstancePublicPorts
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance for which you want to open the public
          ports
        type: string
      - in: query
        name: portInfo
        description: An array of key-value pairs containing information about the
          port mappings
        type: string
      responses:
        200:
          description: OK
      tags:
      - instances
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