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
  /?Action=PeerVpc&k=1:
    get:
      summary: ' Peer Vpc '
      description: Tries to peer the Lightsail VPC with the user's default VPC
      operationId: peerVpc
      parameters:
      - in: query
        name: operation
        description: An array of key-value pairs containing information about the
          request      operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - vpc
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