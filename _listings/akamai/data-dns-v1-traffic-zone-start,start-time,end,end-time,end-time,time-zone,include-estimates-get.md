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
  /data-dns/v1/traffic/{zone}{?start,start_time,end,end_time,end_time,time_zone,include_estimates}:
    get:
      summary: Get Traffic Report
      description: Get Traffic Report
      operationId: datadnsv1trafficzonestartstart-timeendend-timeend-timetime-zoneinclude-estimates
      parameters:
      - in: String
        name: end
        description: End date, in yyyymmdd format
        type: string
      - in: String
        name: end_time
        description: End time, in HH:mm format
        type: string
      - in: Boolean
        name: include_estimates
        description: Flag to include estimated data
        type: string
      - in: String
        name: start
        description: Start date, in yyyymmdd format
        type: string
      - in: String
        name: start_time
        description: Start time, in HH:mm format
        type: string
      - in: String
        name: time_zone
        description: Timezone to use when formatting result set
        type: string
      - in: String
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