---
swagger: "2.0"
info:
  title: Akamai API Get Traffic Report
  description: Get Traffic Report
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /data-dns/v1/traffic/{zone}:
    get:
      summary: Get Traffic Report
      description: Get Traffic Report
      operationId: datadnsv1trafficzonestartstart-timeendend-timeend-timetime-zoneinclude-estimates
      parameters:
      - in: query
        name: end
        description: End date, in yyyymmdd format
        type: string
      - in: query
        name: end_time
        description: End time, in HH:mm format
        type: string
      - in: query
        name: include_estimates
        description: Flag to include estimated data
        type: string
      - in: query
        name: start
        description: Start date, in yyyymmdd format
        type: string
      - in: query
        name: start_time
        description: Start time, in HH:mm format
        type: string
      - in: query
        name: time_zone
        description: Timezone to use when formatting result set
        type: string
      - in: query
        name: zone
        description: Name of Zone
        type: string
      responses:
        200:
          description: OK
      tags:
      - data
      - dns
      - traffic
      - zone
      - start
      - start
      - time
      - end
      - end
      - time
      - end
      - time
      - zone
      - estimates
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