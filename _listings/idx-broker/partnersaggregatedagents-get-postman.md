{
  "info": {
    "name": "IDX Broker Get Partners Aggregated Agents",
    "_postman_id": "6dd8927f-1cd2-4cba-845b-81fe9c0e414b",
    "description": "Get a list of all agents for your clients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Agents",
      "item": [
        {
          "id": "3b016999-c561-4dfc-8237-76fadb60876e",
          "name": "ClientsAgentsGet",
          "request": {
            "url": "http://example.com/clients/agents",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "View agent information on a multi-user account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a67530de-cd7d-436d-ac63-9c8320933b8a"
            }
          ]
        }
      ]
    },
    {
      "name": "Partners",
      "item": [
        {
          "id": "2df6bc77-d4e1-4940-8ce9-362564c59ce9",
          "name": "PartnersAggregatedagentsGet",
          "request": {
            "url": "http://example.com/partners/aggregatedagents",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all agents for your clients."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe20daca-0988-4845-b784-0a0503e1567f"
            }
          ]
        }
      ]
    }
  ]
}