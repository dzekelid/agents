---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 0
info:
  title: AWS OpsWorks API Describe Agent Versions
  version: 1.0.0
  description: Describes the available AWS OpsWorks Stacks agent versions.
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