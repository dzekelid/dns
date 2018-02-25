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
  /?Action=DownloadDefaultKeyPair&k=1:
    get:
      summary: ' Download Default Key Pair '
      description: Downloads the default SSH key pair from the user's account
      operationId: downloadDefaultKeyPair
      parameters:
      - in: query
        name: privateKeyBase64
        description: A base64-encoded RSA private key
        type: string
      - in: query
        name: publicKeyBase64
        description: A base64-encoded public key of the ssh-rsa type
        type: string
      responses:
        200:
          description: OK
      tags:
      - key pairs
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