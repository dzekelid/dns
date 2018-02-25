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
  filterParams:
    get:
      summary: Get Download Delivery Data
      description: Get Download Delivery Data
      operationId: filterparams
      parameters:
      - in: String
        name: aggregation
        description: The aggregation in which the data is required to be grouped
        type: string
      - in: String
        name: cpcodes
        description: Comma-separated CP codes for which the data is required
        type: string
      - in: String
        name: deliveryFormat
        description: One of sp_hds, sp_hls, hls, smooth, others, or all for stream
          packaging HDS, stream packaging HLS, HLS, microsoft smooth streaming, other
          formats and all formats respectively
        type: string
      - in: String
        name: deliveryOption
        description: 'One of the following values: http for non-secure traffic, ssl
          for secure traffic (Shared Certificate), essl for secure traffic (Customer
          Certificate), or all'
        type: string
      - in: String
        name: deliveryType
        description: One of live, vod, or all
        type: string
      - in: String
        name: dimensions
        description: Comma-separated IDs of required dimensions
        type: string
      - in: String
        name: endDate
        description: The end date string in format mm/dd/yyyy:HH:MM
        type: string
      - in: String
        name: filterParams
        description: The UTF&#8211;8 URL-encoded JSON string of the filter parameters
          based on which the data is filtered
        type: string
      - in: String
        name: ipVersion
        description: One of ipv4, ipv6, or all
        type: string
      - in: Number
        name: limit
        description: The number of rows to return
        type: string
      - in: String
        name: metrics
        description: Comma-separated IDs of required metrics
        type: string
      - in: Number
        name: offset
        description: The offset of the row from which the data should start
        type: string
      - in: String
        name: sortParams
        description: The UTF&#8211;8 URL-encoded JSON string of the sort parameters
          based on which the data is sorted
        type: string
      - in: String
        name: startDate
        description: The start date string in format mm/dd/yyyy:HH:MM
        type: string
      - in: String
        name: streams
        description: Comma-separated Stream IDs for which the data is required
        type: string
      responses:
        200:
          description: OK
      tags:
      - filterparams
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