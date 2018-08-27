swagger: "2.0"
x-collection-name: VMWare
x-complete: 1
info:
  title: vRealize Operations 6
  description: todo-add-description
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