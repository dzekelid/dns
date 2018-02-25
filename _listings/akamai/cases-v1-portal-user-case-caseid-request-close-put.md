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
  /cases/v1/portal-user/case/{caseId}/request-close:
    put:
      summary: Close a Request
      description: Close a Request
      operationId: casesv1portalusercasecaseidrequestclose
      parameters:
      - in: String
        name: caseId
        description: Unique identifier for the support ticket
        type: string
      responses:
        200:
          description: OK
      tags:
      - cases
      - v1
      - portal
      - user
      - case
      - case
      - request
      - close
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