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
  /?Action=RegisterCrossAccountAccessRole&k=1:
    get:
      summary: ' Register Cross Account Access Role '
      description: |-
        Registers the IAM role that Amazon Inspector uses to list your EC2 instances at the
                 start of the assessment run or when you call the
      operationId: registerCrossAccountAccessRole
      parameters:
      - in: query
        name: roleArn
        description: The ARN of the IAM role that Amazon Inspector uses to list your
          EC2 instances during         the assessment run or when you call the PreviewAgents
          action
        type: string
      responses:
        200:
          description: OK
      tags:
      - cross account access roles
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