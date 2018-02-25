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
  /cloudlets/api/v2/{policyId}/properties:
    get:
      summary: Get Associated Properties for a Policy
      description: Get Associated Properties for a Policy
      operationId: cloudletsapiv2policyidproperties
      parameters:
      - in: Number
        name: policyId
        description: The ID of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - cloudlets
      - api
      - v2
      - policy
      - properties
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