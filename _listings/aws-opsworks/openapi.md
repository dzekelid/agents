swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAgentVersions:
    get:
      summary: Describe Agent Versions
      description: Describes the available AWS OpsWorks Stacks agent versions.
      operationId: describeAgentVersions
      x-api-path-slug: actiondescribeagentversions-get
      parameters:
      - in: query
        name: ConfigurationManager
        description: The configuration manager
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Agent
      - Versions