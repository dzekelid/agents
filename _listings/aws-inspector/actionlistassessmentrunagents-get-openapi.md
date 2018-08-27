---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API List Assessment Run Agents
  version: 1.0.0
  description: |-
    Lists the agents of the assessment runs that are specified by the ARNs of the
             assessment runs.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PreviewAgents:
    get:
      summary: Preview Agents
      description: |-
        Previews the agents installed on the EC2 instances that are part of the specified
                 assessment target.
      operationId: previewAgents
      x-api-path-slug: actionpreviewagents-get
      parameters:
      - in: query
        name: maxResults
        description: You can use this parameter to indicate the maximum number of
          items you want in the         response
        type: string
      - in: query
        name: nextToken
        description: You can use this parameter when paginating results
        type: string
      - in: query
        name: previewAgentsArn
        description: The ARN of the assessment target whose agents you want to preview
        type: string
      responses:
        200:
          description: OK
      tags:
      - Agents
  /?Action=ListAssessmentRunAgents:
    get:
      summary: List Assessment Run Agents
      description: |-
        Lists the agents of the assessment runs that are specified by the ARNs of the
                 assessment runs.
      operationId: listAssessmentRunAgents
      x-api-path-slug: actionlistassessmentrunagents-get
      parameters:
      - in: query
        name: assessmentRunArn
        description: The ARN that specifies the assessment run whose agents you want
          to list
        type: string
      - in: query
        name: filter
        description: You can use this parameter to specify a subset of data to be
          included in the actions         response
        type: string
      - in: query
        name: maxResults
        description: You can use this parameter to indicate the maximum number of
          items that you want in         the response
        type: string
      - in: query
        name: nextToken
        description: You can use this parameter when paginating results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Run Agents
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