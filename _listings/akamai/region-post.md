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
  region:
    post:
      summary: Submit Load Data
      description: Submit Load Data
      operationId: region
      parameters:
      - in: Number
        name: datacenterId
        description: The ID number for the datacenter (traffic target), from the &#8220;Akamai
          code&#8221; field in the Luna Control Center
        type: string
      - in: String
        name: domain
        description: The name of the GTM domain
        type: string
      - in: String
        name: resource
        description: The name of the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - region
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