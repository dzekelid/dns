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
  /cloudlets/api/v2/policies/{policyId}/versions/{version}{?matchRuleFormat}:
    put:
      summary: Update a Policy Version
      description: Update a Policy Version
      operationId: cloudletsapiv2policiespolicyidversionsversionmatchruleformat
      parameters:
      - in: String
        name: matchRuleFormat
        description: Returns the matchRuleFormat version string, which shows the version
          of the Cloudlet-specific matchRules used
        type: string
      - in: Number
        name: policyId
        description: The ID of the policy
        type: string
      - in: Number
        name: version
        description: The version number of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - cloudlets
      - api
      - v2
      - policies
      - policy
      - versions
      - version
      - matchruleformat
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