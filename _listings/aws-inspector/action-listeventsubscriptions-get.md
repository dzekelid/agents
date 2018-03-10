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
  /?Action=ListEventSubscriptions&k=1:
    get:
      summary: ' List Event Subscriptions '
      description: |-
        Lists all the event subscriptions for the assessment template that is specified by
                 the ARN of the assessment template
      operationId: listEventSubscriptions
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
        name: resourceArn
        description: The ARN of the assessment template for which you want to list
          the existing event         subscriptions
        type: string
      responses:
        200:
          description: OK
      tags:
      - event subscriptions
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