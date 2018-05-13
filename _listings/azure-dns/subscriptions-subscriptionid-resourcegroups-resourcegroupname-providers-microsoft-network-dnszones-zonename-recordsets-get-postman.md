{
  "info": {
    "name": "Azure DNS API Record Sets List By Dns Zone",
    "_postman_id": "d6248e74-27d1-43d0-9a20-fa419df4e8e0",
    "description": "Lists all record sets in a DNS zone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "record sets dns zone",
      "item": [
        {
          "id": "52a85163-0bcd-426c-8aa9-6fc449ea4d64",
          "name": "RecordSets_ListByDnsZone",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/dnsZones/:zoneName/recordsets"
              ],
              "query": [
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "zoneName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all record sets in a DNS zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96c031bc-747a-4577-9a51-5b726e23a993"
            }
          ]
        }
      ]
    }
  ]
}