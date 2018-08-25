---
swagger: "2.0"
x-collection-name: Runscope
x-complete: 1
info:
  title: Runscope
  description: manage-runscope-programmatically-
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{teamId}/agents:
    get:
      summary: Get Teams Agents
      description: Team agents list
      operationId: teams.teamId.agents.get
      x-api-path-slug: teamsteamidagents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Agents
---