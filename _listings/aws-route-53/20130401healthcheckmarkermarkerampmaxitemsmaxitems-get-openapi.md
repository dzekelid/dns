---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 0
info:
  title: AWS Route 53 API List Health Checks
  version: 1.0.0
  description: Retrieve a list of your health checks. Send a GET request to the/2013-04-01/healthcheck
    resource. The response to this request includes aHealthChecks element with zero
    or more HealthCheck child elements.By default, the list of health checks is displayed
    on a single page. You can control thelength of the page that is displayed by using
    the MaxItems parameter. You can usethe Marker parameter to control the health
    check that the list beginswith.For information about listing health checks using
    the Amazon Route 53 console, see Amazon Route 53 Health Checks and DNS Failover.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /2013-04-01/testdnsanswer&amp;edns0clientsubnetip=EDNS0ClientSubnetIP&amp;edns0clientsubnetmask=EDNS0ClientSubnetMask?hostedzoneid=HostedZoneId&amp;recordname=RecordName&amp;recordtype=RecordType&amp;resolverip=ResolverIP
  : get:
      summary: Test D N S Answer
      description: Gets the value that Amazon Route 53 returns in response to a DNS
        request for a specified record name and type. You can optionally specify the
        IP address of a DNS resolver, an EDNS0 client subnet IP address, and a subnet
        mask.
      operationId: testdnsanswer
      x-api-path-slug: 20130401testdnsanswerampedns0clientsubnetipedns0clientsubnetipampedns0clientsubnetmaskedns0clientsubnetmaskhostedzoneidhostedzoneidamprecordnamerecordnameamprecordtyperecordtypeampresolveripresolverip-get
      parameters:
      - in: path
        name: edns0clientsubnetip
        description: If the resolver that you specified for resolverip supports EDNS0,
          specify the IP address of a client in the applicable location
        type: string
      responses:
        200:
          description: OK
      tags:
      - DNS
  /2013-04-01/change/Id:
    get:
      summary: Get Change
      description: 'Returns the current status of a change batch request. The status
        is one of thefollowing values:                  PENDING indicates that the
        changes in this request have not replicatedto all Amazon Route 53 DNS servers.
        This is the initial status of all change batchrequests.                  INSYNC
        indicates that the changes have replicated to all Amazon Route 53 DNSservers.'
      operationId: getchange
      x-api-path-slug: 20130401changeid-get
      parameters:
      - in: path
        name: Id
        description: The ID of the change batch request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Changes
  /2013-04-01/healthcheck/HealthCheckId:
    delete:
      summary: Delete Health Check
      description: Deletes a health check. Send a DELETE request to the/2013-04-01/healthcheck/health
        check ID            resource.ImportantAmazon Route 53 does not prevent you
        from deleting a health check even if the health check isassociated with one
        or more resource record sets. If you delete a health check and you don'tupdate
        the associated resource record sets, the future status of the health check
        can't bepredicted and may change. This will affect the routing of DNS queries
        for your DNS failoverconfiguration. For more information, see Replacing and
        Deleting Health Checks in the Amazon Route 53 Developer Guide.
      operationId: deletehealthcheck
      x-api-path-slug: 20130401healthcheckhealthcheckid-delete
      parameters:
      - in: path
        name: HealthCheckId
        description: The ID of the health check that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
    get:
      summary: Get Health Check
      description: Gets information about a specified health check. Send a GET request
        to the/2013-04-01/healthcheck/health check ID             resource. Formore
        information about using the console to perform this operation, see Amazon
        Route 53 Health Checks and DNS Failover in theAmazon Route 53 Developer Guide.
      operationId: gethealthcheck
      x-api-path-slug: 20130401healthcheckhealthcheckid-get
      parameters:
      - in: path
        name: HealthCheckId
        description: The identifier that Amazon Route 53 assigned to the health check
          when you created it
        type: string
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
  /2013-04-01/healthcheck?marker=Marker&amp;maxitems=MaxItems:
    get:
      summary: List Health Checks
      description: Retrieve a list of your health checks. Send a GET request to the/2013-04-01/healthcheck
        resource. The response to this request includes aHealthChecks element with
        zero or more HealthCheck child elements.By default, the list of health checks
        is displayed on a single page. You can control thelength of the page that
        is displayed by using the MaxItems parameter. You can usethe Marker parameter
        to control the health check that the list beginswith.For information about
        listing health checks using the Amazon Route 53 console, see Amazon Route
        53 Health Checks and DNS Failover.
      operationId: listhealthchecks
      x-api-path-slug: 20130401healthcheckmarkermarkerampmaxitemsmaxitems-get
      parameters:
      - in: path
        name: marker
        description: If the response to a ListHealthChecks is more than one page,
          marker is thehealth check ID for the first health check on the next page
          of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
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