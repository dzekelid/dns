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
  /events/v2/{accountId}/events{?startRange,endRange,sortField,sortOrder,startIndex,limit,customerEventId}:
    put:
      summary: PUT a New Event
      description: PUT a New Event
      operationId: eventsv2accountideventsstartrangeendrangesortfieldsortorderstartindexlimitcustomereventid
      parameters:
      - in: String
        name: accountId
        description: Unique identifier for the account
        type: string
      - in: String
        name: customerEventId
        description: Event identifier for your own use
        type: string
      - in: Number
        name: endRange
        description: End of event, specified as epoch time milliseconds
        type: string
      - in: Number
        name: limit
        description: The maximum number of pagination records to include
        type: string
      - in: String
        name: sortField
        description: The field that should be used to sort the result set
        type: string
      - in: String
        name: sortOrder
        description: The direction of the sort, asc for ascending or desc for descending
        type: string
      - in: Number
        name: startIndex
        description: The zero-origin index at which to start the batch of paginated
          results
        type: string
      - in: Number
        name: startRange
        description: Start of event, specified as epoch time milliseconds
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
      - v2
      - account
      - events
      - startrange
      - endrange
      - sortfield
      - sortorder
      - startindex
      - limit
      - customerevent
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