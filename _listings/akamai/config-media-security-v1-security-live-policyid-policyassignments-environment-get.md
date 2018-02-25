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
  /config-media-security/v1/security/live/{policyID}/policyassignments/{environment}:
    get:
      summary: Get a Policy Assignment
      description: Get a Policy Assignment
      operationId: configmediasecurityv1securitylivepolicyidpolicyassignmentsenvironment
      parameters:
      - in: Enumeration
        name: environment
        description: The environment
        type: string
      - in: Number
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - config
      - media
      - security
      - v1
      - security
      - live
      - policy
      - policyassignments
      - environment
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