---
swagger: "2.0"
info:
  title: AWS Inspector API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeResourceGroups&k=1:
    get:
      summary: ' Describe Resource Groups '
      description: |-
        Describes the resource groups that are specified by the ARNs of the resource
                 groups
      operationId: describeResourceGroups
      parameters:
      - in: query
        name: resourceGroupArns
        description: The ARN that specifies the resource group that you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - resource groups
definitions: []
x-collection-name: AWS Inspector
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