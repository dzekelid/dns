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
  /papi/v0/properties/{propertyId}/versions/{?contractId,groupId}:
    get:
      summary: List Property Versions
      description: List Property Versions
      operationId: papiv0propertiespropertyidversionscontractidgroupid
      parameters:
      - in: String
        name: contractId
        description: Unique identifier for the contract
        type: string
      - in: String
        name: groupId
        description: Unique identifier for the group
        type: string
      - in: String
        name: propertyId
        description: Unique identifier for the property
        type: string
      responses:
        200:
          description: OK
      tags:
      - papi
      - v0
      - properties
      - property
      - versions
      - contract
      - group
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