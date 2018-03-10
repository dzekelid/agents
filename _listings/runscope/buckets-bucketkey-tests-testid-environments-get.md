---
swagger: "2.0"
info:
  title: Runscope
  description: Manage Runscope programmatically.
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /buckets/{bucketKey}/tests/{testId}/environments:
    get:
      summary: Get Buckets Tests Environments
      description: Return details of the test's environments (only those that belong
        to the specified test)
      operationId: buckets.bucketKey.tests.testId.environments.get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - buckets
      - tests
      - environments
definitions:
  Account:
    properties:
      email:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      teams:
        description: This is a default description.
        type: get
  Agent:
    properties:
      agent_id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      version:
        description: This is a default description.
        type: get
  Assertion:
    properties:
      comparison:
        description: This is a default description.
        type: get
      source:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  Bucket:
    properties:
      auth_token:
        description: This is a default description.
        type: get
      collections_url:
        description: This is a default description.
        type: get
      default:
        description: This is a default description.
        type: get
      key:
        description: This is a default description.
        type: get
      messages_url:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      tests_url:
        description: This is a default description.
        type: get
      trigger_url:
        description: This is a default description.
        type: get
      verify_ssl:
        description: This is a default description.
        type: get
  Environment:
    properties:
      auth:
        description: This is a default description.
        type: get
      client_certificate:
        description: This is a default description.
        type: get
      emails:
        description: This is a default description.
        type: get
      exported_at:
        description: This is a default description.
        type: get
      headers:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      initial_script_hash:
        description: This is a default description.
        type: get
      initial_variables:
        description: This is a default description.
        type: get
      integrations:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  Error:
    properties:
      code:
        description: This is a default description.
        type: get
      fields:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  Error400:
    properties:
      error:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      more_info:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
  Integration:
    properties:
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      uuid:
        description: This is a default description.
        type: get
  Meta:
    properties:
      status:
        description: This is a default description.
        type: get
  Metrics:
    properties:
      changes_from_last_period:
        description: This is a default description.
        type: get
      environment_uuid:
        description: This is a default description.
        type: get
      region:
        description: This is a default description.
        type: get
      response_times:
        description: This is a default description.
        type: get
      this_time_period:
        description: This is a default description.
        type: get
      timeframe:
        description: This is a default description.
        type: get
  NewBucket:
    properties:
      name:
        description: This is a default description.
        type: get
      team_id:
        description: This is a default description.
        type: get
  NewMessage:
    properties:
      request:
        description: This is a default description.
        type: get
      response:
        description: This is a default description.
        type: get
  Schedule:
    properties:
      environment_id:
        description: This is a default description.
        type: get
      exported_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      interval:
        description: This is a default description.
        type: get
      note:
        description: This is a default description.
        type: get
      version:
        description: This is a default description.
        type: get
  StandardError:
    properties:
      data:
        description: This is a default description.
        type: get
  Team:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  Test:
    properties:
      created_at:
        description: This is a default description.
        type: get
      created_by:
        description: This is a default description.
        type: get
      default_environment_id:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      last_run:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      trigger_url:
        description: This is a default description.
        type: get
  TestStep:
    properties:
      step_type:
        description: This is a default description.
        type: get
  Variable:
    properties:
      name:
        description: This is a default description.
        type: get
      property:
        description: This is a default description.
        type: get
      source:
        description: This is a default description.
        type: get
x-collection-name: Runscope
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