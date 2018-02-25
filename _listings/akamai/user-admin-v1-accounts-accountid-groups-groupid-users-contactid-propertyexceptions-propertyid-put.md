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
  /user-admin/v1/accounts/{accountId}/groups/{groupId}/users/{contactId}/propertyExceptions/{propertyId}:
    put:
      summary: Modify a Property Exception
      description: Modify a Property Exception
      operationId: useradminv1accountsaccountidgroupsgroupiduserscontactidpropertyexceptionspropertyid
      parameters:
      - in: String
        name: accountId
        description: Unique identifier for an account
        type: string
      - in: String
        name: contactId
        description: Unique identifier for a user
        type: string
      - in: Integer
        name: groupId
        description: Unique numeric identifier for a group
        type: string
      - in: String
        name: propertyId
        description: Within the User Admin API, the assetId is also known as the propertyId
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
      - users
      - contact
      - propertyexceptions
      - property
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