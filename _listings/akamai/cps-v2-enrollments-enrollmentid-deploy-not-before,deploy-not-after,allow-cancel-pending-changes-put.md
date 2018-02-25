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
  /cps/v2/enrollments/{enrollmentId}{?deploy-not-before,deploy-not-after,allow-cancel-pending-changes}:
    put:
      summary: Update an Enrollment
      description: Update an Enrollment
      operationId: cpsv2enrollmentsenrollmentiddeploynotbeforedeploynotafterallowcancelpendingchanges
      parameters:
      - in: Boolean
        name: allow-cancel-pending-changes
        description: When enabled, allows this update to cancel and replace in-process
          changes
        type: string
      - in: String
        name: deploy-not-after
        description: The latest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: String
        name: deploy-not-before
        description: The earliest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: Number
        name: enrollmentId
        description: Integer identifier for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - cps
      - v2
      - enrollments
      - enrollment
      - deploy
      - not
      - before
      - deploy
      - not
      - after
      - allow
      - cancel
      - pending
      - changes
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