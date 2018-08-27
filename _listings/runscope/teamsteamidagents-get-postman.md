{
  "info": {
    "name": "Runscope",
    "_postman_id": "ca424d36-d83d-4c08-b184-4eac7247e8e3",
    "description": "Manage Runscope programmatically.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "teams",
      "item": [
        {
          "id": "c63a85a1-dc52-43a4-b29a-c71d059a2212",
          "name": "teams.teamId.agents.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "teams/:teamId/agents"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "teamId",
                  "value": "teamId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Team agents list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5924072e-9a6c-4647-a3aa-08912052b576"
            }
          ]
        }
      ]
    }
  ]
}