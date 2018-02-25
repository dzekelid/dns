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
  /network-list/v1/network_lists/{networkListId}/history{?sync%2dpoint,extended}:
    get:
      summary: Get Activation Snapshot
      description: Get Activation Snapshot
      operationId: networklistv1network-listsnetworklistidhistorysync2dpointextended
      parameters:
      - in: Boolean
        name: extended
        description: If enabled, returns more verbose data such as creation date and
          activation status
        type: string
      - in: String
        name: networkListId
        description: Unique identifier for the network list, corresponding to the
          unique-id within the data
        type: string
      - in: Number
        name: sync%2dpoint
        description: Indicates how many times the network list has been modified
        type: string
      responses:
        200:
          description: OK
      tags:
      - network
      - list
      - v1
      - network
      - lists
      - networklist
      - history
      - sync%2dpoint
      - extended
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