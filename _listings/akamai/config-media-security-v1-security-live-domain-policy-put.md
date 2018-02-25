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
  /config-media-security/v1/security/live/{domain}/policy:
    put:
      summary: Modify an HD Config Policy
      description: Modify an HD Config Policy
      operationId: configmediasecurityv1securitylivedomainpolicy
      parameters:
      - in: String
        name: domain
        description: The fully qualified domain name for the host in question
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
      - domain
      - policy
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