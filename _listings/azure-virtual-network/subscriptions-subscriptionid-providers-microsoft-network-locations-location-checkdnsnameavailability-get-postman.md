{
  "info": {
    "name": "Azure Virtual Network API Check Dns Name Availability",
    "_postman_id": "85452a25-6313-4c11-95bd-b63fe814ff5f",
    "description": "Checks whether a domain name in the cloudapp.net zone is available for use.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "dns name availability",
      "item": [
        {
          "id": "e092c7af-6414-4940-b454-877c9d90c4a6",
          "name": "CheckDnsNameAvailability",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Network/locations/:location/CheckDnsNameAvailability"
              ],
              "query": [
                {
                  "key": "domainNameLabel",
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
                  "id": "location",
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
            "description": "Checks whether a domain name in the cloudapp"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75cc7b14-9e1c-4ce5-900a-4920964efbe0"
            }
          ]
        }
      ]
    }
  ]
}