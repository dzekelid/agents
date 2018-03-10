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
  /?Action=UnsubscribeFromEvent&k=1:
    get:
      summary: ' Unsubscribe From Event '
      description: |-
        Disables the process of sending Amazon Simple Notification Service (SNS)
                 notifications about a specified event to a specified SNS topic
      operationId: unsubscribeFromEvent
      parameters:
      - in: query
        name: event
        description: The event for which you want to stop receiving SNS notifications
        type: string
      - in: query
        name: resourceArn
        description: The ARN of the assessment template that is used during the event
          for which you want         to stop receiving SNS notifications
        type: string
      - in: query
        name: topicArn
        description: The ARN of the SNS topic to which SNS notifications are sent
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