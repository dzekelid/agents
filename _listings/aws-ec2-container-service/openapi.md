---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 1
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
  /?Action=UpdateContainerAgent:
    get:
      summary: Update Container Agent
      description: Updates the Amazon ECS container agent on a specified container
        instance.
      operationId: updateContainerAgent
      x-api-path-slug: actionupdatecontaineragent-get
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
      - Containers
      - Agents
---