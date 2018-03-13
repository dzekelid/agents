---
swagger: "2.0"
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateContainerAgent&k=1:
    get:
      summary: ' Update Container Agent '
      description: Updates the Amazon ECS container agent on a specified container
        instance
      operationId: updateContainerAgent
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that your container instance is            running on
        type: string
      - in: query
        name: containerInstance
        description: The container instance ID or full Amazon Resource Name (ARN)
          entries for the container instance on            which you would like to
          update the Amazon ECS container agent
        type: string
      responses:
        200:
          description: OK
      tags:
      - container agents
definitions: []
x-collection-name: AWS EC2 Container Service
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