---
swagger: "2.0"
info:
  title: DnsManagementClient
  description: The DNS Management Client.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}
  : patch:
      summary: Record Sets Update
      description: Updates a record set within a DNS zone
      operationId: RecordSets_Update
      parameters:
      - in: header
        name: If-Match
        description: The etag of the record set
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to the Update operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: recordType
        description: The type of DNS record in this record set
      - in: path
        name: relativeRecordSetName
        description: The name of the record set, relative to the name of the zone
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: zoneName
        description: The name of the DNS zone (without a terminating dot)
      responses:
        200:
          description: OK
      tags:
      - record sets
definitions:
  ARecord:
    properties:
      ipv4Address:
        description: This is a default description.
        type: get
  AaaaRecord:
    properties:
      ipv6Address:
        description: This is a default description.
        type: get
  MxRecord:
    properties:
      preference:
        description: This is a default description.
        type: get
      exchange:
        description: This is a default description.
        type: get
  NsRecord:
    properties:
      nsdname:
        description: This is a default description.
        type: get
  PtrRecord:
    properties:
      ptrdname:
        description: This is a default description.
        type: get
  SrvRecord:
    properties:
      priority:
        description: This is a default description.
        type: get
      weight:
        description: This is a default description.
        type: get
      port:
        description: This is a default description.
        type: get
      target:
        description: This is a default description.
        type: get
  TxtRecord:
    properties:
      value:
        description: This is a default description.
        type: get
  CnameRecord:
    properties:
      cname:
        description: This is a default description.
        type: get
  SoaRecord:
    properties:
      host:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      serialNumber:
        description: This is a default description.
        type: get
      refreshTime:
        description: This is a default description.
        type: get
      retryTime:
        description: This is a default description.
        type: get
      expireTime:
        description: This is a default description.
        type: get
      minimumTTL:
        description: This is a default description.
        type: get
  RecordSetProperties:
    properties:
      metadata:
        description: This is a default description.
        type: get
      TTL:
        description: This is a default description.
        type: get
      ARecords:
        description: This is a default description.
        type: get
      AAAARecords:
        description: This is a default description.
        type: get
      MXRecords:
        description: This is a default description.
        type: get
      NSRecords:
        description: This is a default description.
        type: get
      PTRRecords:
        description: This is a default description.
        type: get
      SRVRecords:
        description: This is a default description.
        type: get
      TXTRecords:
        description: This is a default description.
        type: get
  RecordSet:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  RecordSetUpdateParameters:
    properties: []
  RecordSetListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ZoneProperties:
    properties:
      maxNumberOfRecordSets:
        description: This is a default description.
        type: get
      numberOfRecordSets:
        description: This is a default description.
        type: get
      nameServers:
        description: This is a default description.
        type: get
  Zone:
    properties:
      etag:
        description: This is a default description.
        type: get
  ZoneDeleteResult:
    properties:
      azureAsyncOperation:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      statusCode:
        description: This is a default description.
        type: get
      requestId:
        description: This is a default description.
        type: get
  ZoneListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  SubResource:
    properties:
      id:
        description: This is a default description.
        type: get
  CloudError:
    properties: []
  CloudErrorBody:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      target:
        description: This is a default description.
        type: get
      details:
        description: This is a default description.
        type: get
x-collection-name: Azure DNS
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