---
name: Azure DNS
description: Azure DNS lets you host your DNS domains alongside your Azure apps and
  manage DNS records by using your existing Azure subscription. Microsoftrsquo;s global
  network of name servers has the reach, scale, and redundancy to ensure ultra-fast
  DNS responses and ultra-high availability for your domains. With Azure DNS, you
  can be sure your DNS will always be fast and available.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-dns-01-host.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- Microsoft
- DNS
created: "2018-03-13"
modified: "2018-03-13"
url: https://raw.githubusercontent.com/streamdata-gallery/dns/master/_listings/azure-dns/apis.yaml
specificationVersion: "0.14"
apis:
- name: Azure DNS API
  description: Azure DNS lets you host your DNS domains alongside your Azure apps
    and manage DNS records by using your existing Azure subscription
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-dns-01-host.png
  humanURL: ""
  baseURL: ://management.azure.com//
  tags: DNS
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/dns/master/_listings/azure-dns/subscriptions-subscriptionid-resourcegroups-resourcegroupname-providers-microsoft-network-dnszones-zonename-recordsets-get.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/dns/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/dns/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/dns/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/dns/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---