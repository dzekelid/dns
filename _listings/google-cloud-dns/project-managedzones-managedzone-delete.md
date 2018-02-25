---
swagger: "2.0"
info:
  title: Google Cloud DNS
  description: Configures and serves authoritative DNS records.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /dns/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/managedZones/{managedZone}:
    delete:
      summary: Delete Managed Zone
      description: Delete a previously created ManagedZone
      operationId: dns.managedZones.delete
      parameters:
      - in: path
        name: managedZone
        description: Identifies the managed zone addressed by this request
      - in: path
        name: project
        description: Identifies the project addressed by this request
      responses:
        200:
          description: OK
      tags:
      - managed zone
definitions:
  Change:
    properties:
      additions:
        description: This is a default description.
        type: parameters
      deletions:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      startTime:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
  ChangesListResponse:
    properties:
      changes:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  ManagedZone:
    properties:
      creationTime:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      dnsName:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      nameServerSet:
        description: This is a default description.
        type: parameters
      nameServers:
        description: This is a default description.
        type: parameters
  ManagedZonesListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      managedZones:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  Project:
    properties:
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      number:
        description: This is a default description.
        type: parameters
  Quota:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      managedZones:
        description: This is a default description.
        type: parameters
      resourceRecordsPerRrset:
        description: This is a default description.
        type: parameters
      rrsetAdditionsPerChange:
        description: This is a default description.
        type: parameters
      rrsetDeletionsPerChange:
        description: This is a default description.
        type: parameters
      rrsetsPerManagedZone:
        description: This is a default description.
        type: parameters
      totalRrdataSizePerChange:
        description: This is a default description.
        type: parameters
  ResourceRecordSet:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      rrdatas:
        description: This is a default description.
        type: parameters
      ttl:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  ResourceRecordSetsListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      rrsets:
        description: This is a default description.
        type: parameters
x-collection-name: Google Cloud DNS
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