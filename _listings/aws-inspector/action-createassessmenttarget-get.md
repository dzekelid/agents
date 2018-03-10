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
  /?Action=CreateAssessmentTarget&k=1:
    get:
      summary: ' Create Assessment Target '
      description: |-
        Creates a new assessment target using the ARN of the resource group that is generated
                 by
      operationId: createAssessmentTarget
      parameters:
      - in: query
        name: assessmentTargetName
        description: The user-defined name that identifies the assessment target that
          you want to create
        type: string
      - in: query
        name: resourceGroupArn
        description: The ARN that specifies the resource group that is used to create
          the assessment         target
        type: string
      responses:
        200:
          description: OK
      tags:
      - assessment targets
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