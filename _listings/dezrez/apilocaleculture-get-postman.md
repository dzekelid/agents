{
  "info": {
    "name": "Dezrez returns the json file containing localization for the app based on a culture string, and any custom values for the agent",
    "_postman_id": "4d44e07e-1259-4eeb-b12d-147699aeabb2",
    "description": "Returns the json file containing localization for the app based on a culture string, and any custom values for the agent.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "S",
      "item": [
        {
          "id": "991d31e7-0e91-4c0d-a404-220f51436267",
          "name": "AccountingSystem_GetAgentCash",
          "request": {
            "url": "http://api.dezrez.com/api/accountingsystem/agentcash",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Gets overview of the agent cash account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4576cbe-050a-46ce-bf9d-aa0565137888"
            }
          ]
        }
      ]
    },
    {
      "name": "Agent",
      "item": [
        {
          "id": "8a99bd1e-8974-4877-8915-425c4490741f",
          "name": "Invoice_GetAgentFeesEarned",
          "request": {
            "url": "http://api.dezrez.com/api/invoice/fees",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Get agent fees invoices earned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3392d5b2-2ae8-4938-bd60-c26702f79fab"
            }
          ]
        }
      ]
    },
    {
      "name": "Returns",
      "item": [
        {
          "id": "4440b6c4-c9be-443d-8944-51b7c5ee3676",
          "name": "Locale_GetLocalisationFileByculture",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/locale/:culture"
              ],
              "variable": [
                {
                  "id": "culture",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Returns the json file containing localization for the app based on a culture string, and any custom values for the agent."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "325a2d10-3859-42dd-b590-23b5b85dfa1b"
            }
          ]
        }
      ]
    }
  ]
}