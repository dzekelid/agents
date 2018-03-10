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
  /?Action=DescribeRulesPackages&k=1:
    get:
      summary: ' Describe Rules Packages '
      description: |-
        Describes the rules packages that are specified by the ARNs of the rules
                 packages
      operationId: describeRulesPackages
      parameters:
      - in: query
        name: locale
        description: The locale that you want to translate a rules package description
          into
        type: string
      - in: query
        name: rulesPackageArns
        description: The ARN that specifies the rules package that you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - rules packages
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