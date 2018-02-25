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
  /user-admin/v1/accounts/{accountId}/groups/{groupId}/properties:
    get:
      summary: List a Group&#8217;s Properties
      description: List a Group&#8217;s Properties
      operationId: useradminv1accountsaccountidgroupsgroupidproperties
      parameters:
      - in: String
        name: accountId
        description: Unique identifier for an account
        type: string
      - in: Integer
        name: groupId
        description: Unique numeric identifier for a group
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
      - groups
      - group
      - properties
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