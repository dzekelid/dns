---
swagger: "2.0"
info:
  title: Google Site Verification
  description: Verifies ownership of websites or domains with Google.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /siteVerification/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /webResource/{id}:
    delete:
      summary: Relinquish Ownership Of Website
      description: Relinquish ownership of a website or domain
      operationId: siteVerification.webResource.delete
      parameters:
      - in: path
        name: id
        description: The id of a verified site or domain
      responses:
        200:
          description: OK
      tags:
      - website
definitions:
  SiteVerificationWebResourceGettokenRequest:
    properties:
      site:
        description: This is a default description.
        type: put
      verificationMethod:
        description: This is a default description.
        type: put
  SiteVerificationWebResourceGettokenResponse:
    properties:
      method:
        description: This is a default description.
        type: put
      token:
        description: This is a default description.
        type: put
  SiteVerificationWebResourceListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
  SiteVerificationWebResourceResource:
    properties:
      id:
        description: This is a default description.
        type: put
      owners:
        description: This is a default description.
        type: put
      site:
        description: This is a default description.
        type: put
x-collection-name: Google Site Verification
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