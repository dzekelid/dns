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
  /network-list/v1/network_lists{?listType,extended,includeDeprecated,includeElements}:
    get:
      summary: List Network Lists
      description: List Network Lists
      operationId: networklistv1network-listslisttypeextendedincludedeprecatedincludeelements
      parameters:
      - in: Boolean
        name: extended
        description: If enabled, returns more verbose data such as creation date and
          activation status
        type: string
      - in: Boolean
        name: includeDeprecated
        description: When enabled, includes network lists that have been deleted
        type: string
      - in: Boolean
        name: includeElements
        description: When enabled, includes the full list of IP or GEO elements, otherwise
          when disabled only provides high-level data about the network list
        type: string
      - in: String
        name: listType
        description: Filters by the network list type, either GEO or IP
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
      - listtype
      - extended
      - includedeprecated
      - includeelements
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