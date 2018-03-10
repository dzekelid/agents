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
  /?Action=StartAssessmentRun&k=1:
    get:
      summary: ' Start Assessment Run '
      description: Starts the assessment run specified by the ARN of the assessment
        template
      operationId: startAssessmentRun
      parameters:
      - in: query
        name: assessmentRunName
        description: You can specify the name for the assessment run
        type: string
      - in: query
        name: assessmentTemplateArn
        description: The ARN of the assessment template of the assessment run that
          you want to         start
        type: string
      responses:
        200:
          description: OK
      tags:
      - assessment runs
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