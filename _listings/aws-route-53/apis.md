---
name: AWS Route 53
x-slug: aws-route-53
description: Amazon Route 53 is a highly available and scalable cloud Domain Name
  System (DNS) web service. It is designed to give developers and businesses an extremely
  reliable and cost effective way to route end users to Internet applications by translating
  names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers
  use to connect to each other. Amazon Route 53 is fully compliant with IPv6 as well.Amazon
  Route 53 effectively connects user requests to infrastructure running in AWS &ndash;
  such as Amazon EC2 instances, Elastic Load Balancing load balancers, or Amazon S3
  buckets &ndash; and can also be used to route users to infrastructure outside of
  AWS. You can use Amazon Route 53 to configure DNS health checks to route traffic
  to healthy endpoints or to independently monitor the health of your application
  and its endpoints. Amazon Route 53 Traffic Flow makes it easy for you to manage
  traffic globally through a variety of routing types, including Latency Based Routing,
  Geo DNS, and Weighted Round Robin&mdash;all of which can be combined with DNS Failover
  in order to enable a variety of low-latency, fault-tolerant architectures. Using
  Amazon Route 53 Traffic Flow&rsquo;s simple visual editor, you can easily manage
  how your end-users are routed to your application&rsquo;s endpoints&mdash;whether
  in a single AWS region or distributed around the globe. Amazon Route 53 also offers
  Domain Name Registration &ndash; you can purchase and manage domain names such as
  example.com and Amazon Route 53 will automatically configure DNS settings for your
  domains.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
x-kinRank: "8"
x-alexaRank: "0"
tags: DNS
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Route 53 API - Test D N S Answer
  x-api-slug: 20130401testdnsanswerampedns0clientsubnetipedns0clientsubnetipampedns0clientsubnetmaskedns0clientsubnetmaskhostedzoneidhostedzoneidamprecordnamerecordnameamprecordtyperecordtypeampresolveripresolverip-get
  description: Gets the value that Amazon Route 53 returns in response to a DNS request
    for a specified record name and type. You can optionally specify the IP address
    of a DNS resolver, an EDNS0 client subnet IP address, and a subnet mask.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401testdnsanswerampedns0clientsubnetipedns0clientsubnetipampedns0clientsubnetmaskedns0clientsubnetmaskhostedzoneidhostedzoneidamprecordnamerecordnameamprecordtyperecordtypeampresolveripresolverip-get-openapi.md
- name: AWS Route 53 API - Get Change
  x-api-slug: 20130401changeid-get
  description: 'Returns the current status of a change batch request. The status is
    one of thefollowing values:                  PENDING indicates that the changes
    in this request have not replicatedto all Amazon Route 53 DNS servers. This is
    the initial status of all change batchrequests.                  INSYNC indicates
    that the changes have replicated to all Amazon Route 53 DNSservers.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401changeid-get-openapi.md
- name: AWS Route 53 API - Delete Health Check
  x-api-slug: 20130401healthcheckhealthcheckid-delete
  description: Deletes a health check. Send a DELETE request to the/2013-04-01/healthcheck/health
    check ID            resource.ImportantAmazon Route 53 does not prevent you from
    deleting a health check even if the health check isassociated with one or more
    resource record sets. If you delete a health check and you don'tupdate the associated
    resource record sets, the future status of the health check can't bepredicted
    and may change. This will affect the routing of DNS queries for your DNS failoverconfiguration.
    For more information, see Replacing and Deleting Health Checks in the Amazon Route
    53 Developer Guide.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401healthcheckhealthcheckid-delete-openapi.md
- name: AWS Route 53 API - Get Health Check
  x-api-slug: 20130401healthcheckhealthcheckid-get
  description: Gets information about a specified health check. Send a GET request
    to the/2013-04-01/healthcheck/health check ID             resource. Formore information
    about using the console to perform this operation, see Amazon Route 53 Health
    Checks and DNS Failover in theAmazon Route 53 Developer Guide.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401healthcheckhealthcheckid-get-openapi.md
- name: AWS Route 53 API - List Health Checks
  x-api-slug: 20130401healthcheckmarkermarkerampmaxitemsmaxitems-get
  description: Retrieve a list of your health checks. Send a GET request to the/2013-04-01/healthcheck
    resource. The response to this request includes aHealthChecks element with zero
    or more HealthCheck child elements.By default, the list of health checks is displayed
    on a single page. You can control thelength of the page that is displayed by using
    the MaxItems parameter. You can usethe Marker parameter to control the health
    check that the list beginswith.For information about listing health checks using
    the Amazon Route 53 console, see Amazon Route 53 Health Checks and DNS Failover.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401healthcheckmarkermarkerampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - Create Hosted Zone
  x-api-slug: 20130401hostedzone-post
  description: Creates a new public hosted zone, used to specify how the Domain Name
    System (DNS)routes traffic on the Internet for a domain, such as example.com,
    and its subdomains. ImportantPublic hosted zones can't be converted to a private
    hosted zone or vice versa.Instead, create a new hosted zone with the same name
    and create new resource recordsets.Send a POST request to the /2013-04-01/hostedzone
    resource. The request body must include a documentwith a CreateHostedZoneRequest
    element. The response returns theCreateHostedZoneResponse element containing metadata
    about the hostedzone.Fore more information about charges for hosted zones, see
    Amazon Route 53 Pricing.Note the following:You can't create a hosted zone for
    a top-level domain (TLD).Amazon Route 53 automatically creates a default SOA record
    and four NS records for the zone.For more information about SOA and NS records,
    see NS and SOA Records that Amazon Route 53 Creates for a Hosted Zone in the Amazon
    Route 53 Developer Guide.If your domain is registered with a registrar other than
    Amazon Route 53, you must update thename servers with your registrar to make Amazon
    Route 53 your DNS service. For more information, seeConfiguring Amazon Route 53
    as your DNSService in the Amazon Route 53 Developer's Guide.After creating a zone,
    its initial status is PENDING. This means that itis not yet available on all DNS
    servers. The status of the zone changes to INSYNCwhen the NS and SOA records are
    available on all Amazon Route 53 DNS servers. When trying to create a hosted zone
    using a reusable delegation set, specify anoptional DelegationSetId, and Amazon
    Route 53 would assign those 4 NS records for the zone, instead ofallotting a new
    one.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401hostedzone-post-openapi.md
- name: AWS Route 53 API - List Resource Record Sets
  x-api-slug: 20130401hostedzoneidrrsetampidentifierstartrecordidentifierampmaxitemsmaxitemsnamestartrecordnameamptypestartrecordtype-get
  description: 'Lists the resource record sets in a specified hosted zone.            ListResourceRecordSets
    returns up to 100 resource record sets at a time in ASCII order, beginning at
    a position specified by the name and type elements. The action sorts results first
    by DNS name with the labels reversed, for example:            com.example.www.         Note
    the trailing dot, which can change the sort order in some circumstances.When multiple
    records have the same DNS name, the action sorts results by the record type.You
    can use the name and type elements to adjust the beginning position of the list
    of resource record sets returned:If you do not specify Name or TypeThe results
    begin with the first resource record set that the hosted zone contains.If you
    specify Name but not TypeThe results begin with the first resource record set
    in the list whose name is greater than or equal to Name.If you specify Type but
    not NameAmazon Route 53 returns the InvalidInput error.If you specify both Name
    and TypeThe results begin with the first resource record set in the list whose
    name is greater than or equal to Name, and whose type is greater than or equal
    to Type.This action returns the most current version of the records. This includes
    records that are PENDING, and that are not yet available on all Amazon Route 53
    DNS servers.To ensure that you get an accurate listing of the resource record
    sets for a hosted zone at a point in time, do not submit a ChangeResourceRecordSets
    request while you''re paging through the results of a ListResourceRecordSets request.
    If you do, some pages may display results without the latest changes while other
    pages display results with the latest changes.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401hostedzoneidrrsetampidentifierstartrecordidentifierampmaxitemsmaxitemsnamestartrecordnameamptypestartrecordtype-get-openapi.md
- name: AWS Route 53 API - Change Resource Record Sets
  x-api-slug: 20130401hostedzoneidrrset-post
  description: 'Create, change, update, or delete authoritative DNS information on
    all Amazon Route 53 servers.Send a POST request to:             /2013-04-01/hostedzone/Amazon
    Route 53 hosted ZoneID/rrset resource. The request body must include a document
    with aChangeResourceRecordSetsRequest element. The request body contains a list
    ofchange items, known as a change batch. Change batches are considered transactional
    changes.When using the Amazon Route 53 API to change resource record sets, Amazon
    Route 53 either makes all or none of thechanges in a change batch request. This
    ensures that Amazon Route 53 never partially implements theintended changes to
    the resource record sets in a hosted zone. For example, a change batch request
    that deletes the CNAME record forwww.example.com and creates an alias resource
    record set for www.example.com. Amazon Route 53 deletesthe first resource record
    set and creates the second resource record set in a singleoperation. If either
    the DELETE or the CREATE action fails, thenboth changes (plus any other changes
    in the batch) fail, and the original CNAMErecord continues to exist.ImportantDue
    to the nature of transactional changes, you can''t delete the same resourcerecord
    set more than once in a single change batch. If you attempt to delete the same
    changebatch more than once, Amazon Route 53 returns an InvalidChangeBatch error.NoteTo
    create resource record sets for complex routing configurations, use either thetraffic
    flow visual editor in the Amazon Route 53 console or the API actions for traffic
    policies andtraffic policy instances. Save the configuration as a traffic policy,
    then associate thetraffic policy with one or more domain names (such as example.com)
    or subdomain names (suchas www.example.com), in the same hosted zone or in multiple
    hosted zones. You can roll backthe updates if the new configuration isn''t performing
    as expected. For more information, seeUsing Traffic Flow to Route DNSTraffic in
    the Amazon Route 53 Developer Guide.Use ChangeResourceRecordsSetsRequest to perform
    the following actions:                  CREATE: Creates a resource record set
    that has the specified values.                  DELETE: Deletes an existing resource
    record set that has the specified values.                  UPSERT: If a resource
    record set does not already exist, AWS createsit. If a resource set does exist,
    Amazon Route 53 updates it with the values in the request. The values that you
    need to include in the request depend on the type of resource record set that
    you''re creating, deleting, or updating:            Basic resource record sets
    (excluding alias, failover, geolocation, latency, and weighted resource record
    sets)                           Name                                 Type                                 TTL                           Failover,
    geolocation, latency, or weighted resource record sets (excluding alias resource
    record sets)                           Name                                 Type                                 TTL                                 SetIdentifier                           Alias
    resource record sets (including failover alias, geolocation alias, latency alias,
    and weighted alias resource record sets)                           Name                                 Type                                 AliasTarget
    (includes DNSName, EvaluateTargetHealth, and HostedZoneId)                  SetIdentifier
    (for failover, geolocation, latency, and weighted resource record sets)When you
    submit a ChangeResourceRecordSets request, Amazon Route 53 propagates your changes
    to all of the Amazon Route 53 authoritative DNS servers. While your changes are
    propagating, GetChange returns a status of PENDING. When propagation is complete,
    GetChange returns a status of INSYNC. Changes generally propagate to all Amazon
    Route 53 name servers in a few minutes. In rare circumstances, propagation can
    take up to 30 minutes. For more information, see GetChange       For information
    about the limits on a ChangeResourceRecordSets request, see Limits in the Amazon
    Route 53 Developer Guide.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401hostedzoneidrrset-post-openapi.md
- name: AWS Route 53 API - List Hosted Zones By Name
  x-api-slug: 20130401hostedzonesbynamednsnamednsnameamphostedzoneidhostedzoneidampmaxitemsmaxitems-get
  description: 'Retrieves a list of your hosted zones in lexicographic order. Send
    a GETrequest to the /2013-04-01/hostedzonesbyname resource. The response includes
    aHostedZones child element for each hosted zone created by the current AWSaccount.             ListHostedZonesByName
    sorts hosted zones by name with the labels reversed.For example:                  com.example.www.               Note
    the trailing dot, which can change the sort order in some circumstances.If the
    domain name includes escape characters or Punycode,ListHostedZonesByName alphabetizes
    the domain name using the escaped orPunycoded value, which is the format that
    Amazon Route 53 saves in its database. For example, to createa hosted zone for
    example.com, specify ex\344mple.com for the domain name.ListHostedZonesByName
    alphabetizes it as:                  com.ex\344mple.               The labels
    are reversed and alphabetized using the escaped value. For more informationabout
    valid domain name formats, including internationalized domain names, see DNS Domain
    Name Format in theAmazon Route 53 Developer Guide.Amazon Route 53 returns up to
    100 items in each response. If you have a lot of hosted zones, usethe MaxItems
    parameter to list them in groups of up to 100. The response includesvalues that
    help navigate from one group of MaxItems hosted zones to thenext:The DNSName and
    HostedZoneId elements in the responsecontain the values, if any, specified for
    the dnsname andhostedzoneid parameters in the request that produced the currentresponse.The
    MaxItems element in the response contains the value, if any, thatyou specified
    for the maxitems parameter in the request that produced thecurrent response.If
    the value of IsTruncated in the response is true, there are morehosted zones associated
    with the current AWS account. If IsTruncated is false, this response includes
    the last hosted zonethat is associated with the current account. The NextDNSName
    element andNextHostedZoneId elements are omitted from the response.The NextDNSName
    and NextHostedZoneId elements in theresponse contain the domain name and the hosted
    zone ID of the next hosted zone that isassociated with the current AWS account.
    If you want to list more hosted zones, makeanother call to ListHostedZonesByName,
    and specify the value ofNextDNSName and NextHostedZoneId in the dnsnameand hostedzoneid
    parameters, respectively.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401hostedzonesbynamednsnamednsnameamphostedzoneidhostedzoneidampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - Create Traffic Policy
  x-api-slug: 20130401trafficpolicy-post
  description: Creates a traffic policy, which you use to create multiple DNS resource
    record sets forone domain name (such as example.com) or one subdomain name (such
    aswww.example.com).Send a POST request to the /2013-04-01/trafficpolicy resource.
    The request body must include a documentwith a CreateTrafficPolicyRequest element.
    The response includes theCreateTrafficPolicyResponse element, which contains information
    about the newtraffic policy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401trafficpolicy-post-openapi.md
- name: AWS Route 53 API - Create Traffic Policy Version
  x-api-slug: 20130401trafficpolicyid-post
  description: Creates a new version of an existing traffic policy. When you create
    a new version of atraffic policy, you specify the ID of the traffic policy that
    you want to update and aJSON-formatted document that describes the new version.
    You use traffic policies to createmultiple DNS resource record sets for one domain
    name (such as example.com) or one subdomainname (such as www.example.com). You
    can create a maximum of 1000 versions of a traffic policy.If you reach the limit
    and need to create another version, you'll need to start a new trafficpolicy.Send
    a POST request to the /2013-04-01/trafficpolicy/ resource. The request body includes
    a document witha CreateTrafficPolicyVersionRequest element. The response returns
    theCreateTrafficPolicyVersionResponse element, which contains information aboutthe
    new version of the traffic policy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401trafficpolicyid-post-openapi.md
- name: AWS Route 53 API - Create Traffic Policy Instance
  x-api-slug: 20130401trafficpolicyinstance-post
  description: Creates resource record sets in a specified hosted zone based on the
    settings in aspecified traffic policy version. In addition, CreateTrafficPolicyInstanceassociates
    the resource record sets with a specified domain name (such as example.com) orsubdomain
    name (such as www.example.com). Amazon Route 53 responds to DNS queries for the
    domain orsubdomain name by using the resource record sets that CreateTrafficPolicyInstancecreated.Send
    a POST request to the /2013-04-01/trafficpolicyinstance resource. The request
    body must include adocument with a CreateTrafficPolicyRequest element. The response
    returns theCreateTrafficPolicyInstanceResponse element, which contains information
    aboutthe traffic policy instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401trafficpolicyinstance-post-openapi.md
- name: AWS Route 53 API - Update Traffic Policy Instance
  x-api-slug: 20130401trafficpolicyinstanceid-post
  description: Updates the resource record sets in a specified hosted zone that were
    created based onthe settings in a specified traffic policy version.Send a POST
    request to the /2013-04-01/trafficpolicyinstance/traffic policy ID            resource.
    The request body must include a document with anUpdateTrafficPolicyInstanceRequest
    element.When you update a traffic policy instance, Amazon Route 53 continues to
    respond to DNS queriesfor the root resource record set name (such as example.com)
    while it replaces one group ofresource record sets with another. Amazon Route
    53 performs the following operations:Amazon Route 53 creates a new group of resource
    record sets based on the specified trafficpolicy. This is true regardless of how
    substantial the differences are between theexisting resource record sets and the
    new resource record sets. When all of the new resource record sets have been created,
    Amazon Route 53 starts to respondto DNS queries for the root resource record set
    name (such as example.com) by using thenew resource record sets.Amazon Route 53
    deletes the old group of resource record sets that are associated with theroot
    resource record set name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dns/master/_listings/aws-route-53/20130401trafficpolicyinstanceid-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.rekognition.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.route.53.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/Route53/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/route53/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=87
- type: x-pricing
  url: https://aws.amazon.com/route53/pricing/
- type: x-registrar-policies
  url: https://aws.amazon.com/route53/amazon-registrar-policies/
- type: x-service-health
  url: http://status.aws.amazon.com/
- type: x-service-level-agreement
  url: https://aws.amazon.com/route53/sla
- type: x-sla
  url: https://aws.amazon.com/route53/sla/
- type: x-website
  url: https://aws.amazon.com/route53/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---