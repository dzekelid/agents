---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Update EP Ops Agent
  description: 'TODO: Add Description'
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /internal/agent/upgrade:
    post:
      summary: Update EP Ops Agent
      description: 'TODO: Add Description'
      operationId: InternalAgentUpgradePost
      x-api-path-slug: internalagentupgrade-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: header
        name: X-vRealizeOps-API-use-unsupported
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Agent
      - Upgrade
  /adapterkinds/EP Ops Adapter/resourcekinds/EP Ops Agent/resources:
    get:
      summary: Get Agent Status on Upgrade
      description: Need agent ID (token)
      operationId: AdapterkindsEPOpsAdapterResourcekindsEPOpsAgentResourcesGet
      x-api-path-slug: adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: identifiers[agentID]
      responses:
        200:
          description: OK
      tags:
      - Adapterkinds
      - EP
      - Ops
      - Adapter
      - Resourcekinds
      - EP
      - Ops
      - Agent
      - Resources
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---