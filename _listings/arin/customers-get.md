---
swagger: "2.0"
info:
  title: Customer API
  description: For managing customers
  version: "1.0"
host: whois.arin.net
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers:
    get:
      summary: Manage customers
      description: ""
      operationId: customers
      parameters:
      - in: query
        name: handle
        description: the handle of the customer
        type: string
        format: string
      - in: query
        name: name
        description: the name of the customer
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - customers
definitions: []
x-collection-name: ARIN
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