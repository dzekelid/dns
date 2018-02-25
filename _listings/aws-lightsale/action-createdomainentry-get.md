---
swagger: "2.0"
info:
  title: AWS Lightsale API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDomainEntry&k=1:
    get:
      summary: ' Create Domain Entry '
      description: |-
        Creates one of the following entry records associated with the domain: A record, CNAME
              record, TXT record, or MX record
      operationId: createDomainEntry
      parameters:
      - in: query
        name: domainEntry
        description: An array of key-value pairs containing information about the
          domain entry      request
        type: string
      - in: query
        name: domainName
        description: The domain name (e
        type: string
      responses:
        200:
          description: OK
      tags:
      - domains
definitions: []
x-collection-name: AWS Lightsale
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