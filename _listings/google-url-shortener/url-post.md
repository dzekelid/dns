---
swagger: "2.0"
info:
  title: URL Shortener
  description: Lets you create, inspect, and manage goo.gl short URLs
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /urlshortener/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /url:
    post:
      summary: Create Short URL
      description: Creates a new short URL
      operationId: urlshortener.url.insert
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - short url
definitions:
  AnalyticsSnapshot:
    properties:
      browsers:
        description: This is a default description.
        type: parameters
      countries:
        description: This is a default description.
        type: parameters
      longUrlClicks:
        description: This is a default description.
        type: parameters
      platforms:
        description: This is a default description.
        type: parameters
      referrers:
        description: This is a default description.
        type: parameters
      shortUrlClicks:
        description: This is a default description.
        type: parameters
  AnalyticsSummary:
    properties: []
  StringCount:
    properties:
      count:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
  Url:
    properties:
      created:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      longUrl:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
  UrlHistory:
    properties:
      items:
        description: This is a default description.
        type: parameters
      itemsPerPage:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      totalItems:
        description: This is a default description.
        type: parameters
x-collection-name: Google URL Shortener
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