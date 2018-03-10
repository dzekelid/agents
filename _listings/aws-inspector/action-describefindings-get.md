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
  /?Action=DescribeFindings&k=1:
    get:
      summary: ' Describe Findings '
      description: Describes the findings that are specified by the ARNs of the findings
      operationId: describeFindings
      parameters:
      - in: query
        name: findingArns
        description: The ARN that specifies the finding that you want to describe
        type: string
      - in: query
        name: locale
        description: The locale into which you want to translate a finding description,
          recommendation,         and the short description that identifies the finding
        type: string
      responses:
        200:
          description: OK
      tags:
      - findings
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