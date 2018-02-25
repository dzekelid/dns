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
  /events/v2/{accountId}/srip{?sortField,sortOrder,limit,startIndex}:
    get:
      summary: List IPA and SXL Configurations
      description: List IPA and SXL Configurations
      operationId: eventsv2accountidsripsortfieldsortorderlimitstartindex
      parameters:
      - in: String
        name: accountId
        description: Unique identifier for the account
        type: string
      - in: Number
        name: limit
        description: The maximum number of pagination records to include
        type: string
      - in: String
        name: sortField
        description: The field to sort the result set, either description or hostname
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
      responses:
        200:
          description: OK
      tags:
      - events
      - v2
      - account
      - srip
      - sortfield
      - sortorder
      - limit
      - startindex
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