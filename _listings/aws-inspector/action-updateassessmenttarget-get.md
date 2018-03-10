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
  /?Action=UpdateAssessmentTarget&k=1:
    get:
      summary: ' Update Assessment Target '
      description: |-
        Updates the assessment target that is specified by the ARN of the assessment
                 target
      operationId: updateAssessmentTarget
      parameters:
      - in: query
        name: assessmentTargetArn
        description: The ARN of the assessment target that you want to update
        type: string
      - in: query
        name: assessmentTargetName
        description: The name of the assessment target that you want to update
        type: string
      - in: query
        name: resourceGroupArn
        description: The ARN of the resource group that is used to specify the new
          resource group to         associate with the assessment target
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