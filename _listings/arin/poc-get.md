---
swagger: "2.0"
info:
  title: Point of Contact (POC) API
  description: For managing Point of Contact (POC).
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /poc:
    get:
      summary: Point of Contact (POC)
      description: lists the Point of Contact (POC)
      operationId: poc
      parameters:
      - in: query
        name: city
        description: the city registered by the POC
        type: string
        format: string
      - in: query
        name: company
        description: the company name registered by the POC
        type: string
        format: string
      - in: query
        name: domain
        description: the domain of the email address for the POC
        type: string
        format: string
      - in: query
        name: first
        description: the first name of the POC
        type: string
        format: string
      - in: query
        name: handle
        description: the handle of the POC
        type: string
        format: string
      - in: query
        name: last
        description: the last name of the POC
        type: string
        format: string
      - in: query
        name: middle
        description: the middle name of the POC
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - point of contact
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