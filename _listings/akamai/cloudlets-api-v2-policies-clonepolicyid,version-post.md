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
  /cloudlets/api/v2/policies{?clonePolicyId,version}:
    post:
      summary: Create a Policy
      description: Create a Policy
      operationId: cloudletsapiv2policiesclonepolicyidversion
      parameters:
      - in: Number
        name: clonePolicyId
        description: If cloning an existing policy, this parameter is the ID of the
          policy (policyId) you want to clone
        type: string
      - in: Number
        name: version
        description: For POST operations, indicates the version of the existing policy
          to use for the new policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - cloudlets
      - api
      - v2
      - policies
      - clonepolicy
      - version
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