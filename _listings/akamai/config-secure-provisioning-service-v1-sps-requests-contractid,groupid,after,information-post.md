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
  /config-secure-provisioning-service/v1/sps-requests{?contractId,groupId,after,information}:
    post:
      summary: Create a Request
      description: Create a Request
      operationId: configsecureprovisioningservicev1spsrequestscontractidgroupidafterinformation
      parameters:
      - in: String
        name: after
        description: If specified for GET requests, returns only the SPS requests
          created after the date entered
        type: string
      - in: Number
        name: contractId
        description: For POST requests, the ID of the contract associated with the
          new policy
        type: string
      - in: Number
        name: groupId
        description: For POST requests, the ID of the group associated with the new
          policy
        type: string
      - in: Boolean
        name: information
        description: If specified for GET requests, returns parameters posted with
          the SPS request resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - config
      - secure
      - provisioning
      - service
      - v1
      - sps
      - requests
      - contract
      - group
      - after
      - information
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