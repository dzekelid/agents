{
  "info": {
    "name": "IDX Broker Get Agents",
    "_postman_id": "2a81da65-9b64-4217-ad1e-bc6d7a1d13bf",
    "description": "View agent information on a multi-user account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Agents",
      "item": [
        {
          "id": "07badd78-a21e-4faa-b257-7a7ba9ceadd0",
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
              "id": "c7b62c26-e0d2-4a75-8847-4b938bba9dcc"
            }
          ]
        }
      ]
    }
  ]
}