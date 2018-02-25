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
  /user-admin/v1/accounts/{accountId}/roles/{roleId}:
    get:
      summary: Get a Role
      description: Get a Role
      operationId: useradminv1accountsaccountidrolesroleid
      parameters:
      - in: String
        name: accountId
        description: Unique identifier for an account
        type: string
      - in: String
        name: roleId
        description: Unique identifier for a role object
        type: string
      responses:
        200:
          description: OK
      tags:
      - user
      - admin
      - v1
      - accounts
      - account
      - roles
      - role
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