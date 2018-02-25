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
  /cases/v1/portal-user{?status,type,category}:
    get:
      summary: List Cases
      description: List Cases
      operationId: casesv1portaluserstatustypecategory
      parameters:
      - in: Enumeration
        name: category
        description: ts for technicalSupport, or etc (currently ignored)
        type: string
      - in: String
        name: status
        description: Retrieves all if missing, both active and closed cases
        type: string
      - in: String
        name: type
        description: Retrieves all if missing, both user and company cases
        type: string
      responses:
        200:
          description: OK
      tags:
      - cases
      - v1
      - portal
      - user
      - status
      - type
      - category
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