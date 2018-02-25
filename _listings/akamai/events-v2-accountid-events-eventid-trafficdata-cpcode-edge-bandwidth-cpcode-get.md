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
  /events/v2/{accountId}/events/{eventId}/trafficdata/cpcode/edge/bandwidth/{cpcode}:
    get:
      summary: Get Edge Bandwidth per CP Code
      description: Get Edge Bandwidth per CP Code
      operationId: eventsv2accountideventseventidtrafficdatacpcodeedgebandwidthcpcode
      parameters:
      - in: String
        name: accountId
        description: Unique identifier for the account
        type: string
      - in: Number
        name: cpcode
        description: The CP code associated with the given event
        type: string
      - in: Number
        name: eventId
        description: Unique identifier for the event
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
      - v2
      - account
      - events
      - event
      - trafficdata
      - cpcode
      - edge
      - bandwth
      - cpcode
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