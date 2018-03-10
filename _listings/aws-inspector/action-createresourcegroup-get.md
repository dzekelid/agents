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
  /?Action=CreateResourceGroup&k=1:
    get:
      summary: ' Create Resource Group '
      description: |-
        Creates a resource group using the specified set of tags (key and value pairs) that
                 are used to select the EC2 instances to be included in an Amazon Inspector assessment
                 target
      operationId: createResourceGroup
      parameters:
      - in: query
        name: resourceGroupTags
        description: A collection of keys and an array of possible values,         '[{key:key1,values:[Value1,Value2]},{key:Key2,values:[Value3]}]'
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