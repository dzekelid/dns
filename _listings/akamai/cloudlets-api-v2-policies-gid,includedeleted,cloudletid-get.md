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
  /cloudlets/api/v2/policies{?gid,includeDeleted,cloudletId}:
    get:
      summary: List Policies
      description: List Policies
      operationId: cloudletsapiv2policiesgidincludedeletedcloudletid
      parameters:
      - in: Number
        name: cloudletId
        description: For GET operations, returns only policies for this particular
          cloudletId
        type: string
      - in: Number
        name: gid
        description: For GET operations, returns only policies associated with the
          group ID (gid) entered
        type: string
      - in: Boolean
        name: includeDeleted
        description: For GET operations, includes deleted policies in the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - cloudlets
      - api
      - v2
      - policies
      - g
      - includedeleted
      - cloudlet
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