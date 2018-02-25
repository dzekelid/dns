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
  deliveryFormat:
    get:
      summary: Get Edge Bandwidth for Universal Live Streams
      description: Get Edge Bandwidth for Universal Live Streams
      operationId: deliveryformat
      parameters:
      - in: String
        name: accountId
        description: Unique identifier for the account
        type: string
      - in: String
        name: deliveryFormat
        description: The stream format, discussed above
        type: string
      - in: Number
        name: eventId
        description: Unique identifier for the event
        type: string
      - in: String
        name: range
        description: The range, in minutes, of data to retrieve
        type: string
      - in: Number
        name: streamId
        description: Unique identifier for the stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - deliveryformat
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