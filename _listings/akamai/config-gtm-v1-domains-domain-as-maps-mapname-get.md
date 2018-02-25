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
  /config-gtm/v1/domains/{domain}/as-maps/{mapName}:
    get:
      summary: Get an AS Map
      description: Get an AS Map
      operationId: configgtmv1domainsdomainasmapsmapname
      parameters:
      - in: String
        name: domain
        description: Name of Traffic Management domain
        type: string
      - in: String
        name: mapName
        description: Name of AS Map to create, update or delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - config
      - gtm
      - v1
      - domains
      - domain
      - as
      - maps
      - mapname
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