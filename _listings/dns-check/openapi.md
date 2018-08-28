swagger: "2.0"
x-collection-name: DNS Check
x-complete: 1
info:
  title: DNS Record Group Monitoring API
  description: a-dns-record-group-is-a-logical-collection-of-dns-records--dns-record-groups-can-have-a-onetoone-correlation-with-zone-files-but-other-types-of-groupings-are-possible-as-well-such-as-grouping-by-service-or-customer--see-the-dns-record-groups-page-for-more-details--the-dns-check-api-is-used-to-request-data-for-either-a-specific-record-group-or-all-dns-record-groups-owned-by-your-account-
  version: v1
host: www.dnscheck.co
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json