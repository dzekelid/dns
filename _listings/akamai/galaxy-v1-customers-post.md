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
  /galaxy/v1/customers:
    post:
      summary: Add a Customer
      description: Add a Customer
      operationId: galaxyv1customers
      parameters:
      - in: String
        name: akamaiCustomerId
        description: Akamai ID of the customer, maximum 50 characters
        type: string
      - in: Boolean
        name: debug
        description: The flag to include debug members in the response JSON
        type: string
      responses:
        200:
          description: OK
      tags:
      - galaxy
      - v1
      - customers
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