---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Utility APIs Update an outcome
  description: Update an outcome.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /outcomes/{id}:
    get:
      summary: Show an outcome
      description: Show an outcome.
      operationId: show-an-outcome
      x-api-path-slug: outcomesid-get
      responses:
        200:
          description: OK
      tags:
      - Outcomes
      - Id
    put:
      summary: Update an outcome
      description: Update an outcome.
      operationId: update-an-outcome
      x-api-path-slug: outcomesid-put
      parameters:
      - in: query
        name: calculation_int
        description: The new calculation int
      - in: query
        name: calculation_method
        description: The new calculation method
      - in: query
        name: description
        description: The new outcome description
      - in: query
        name: display_name
        description: A friendly name shown in reports for outcomes with cryptic titles,
          such asncommon core standards names
      - in: query
        name: mastery_points
        description: The new mastery threshold for the embedded rubric criterion
      - in: query
        name: ratings[][description]
        description: The description of a new rating level for the embedded rubric
          criterion
      - in: query
        name: ratings[][points]
        description: The points corresponding to a new rating level for the embedded
          rubricncriterion
      - in: query
        name: title
        description: The new outcome title
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
      responses:
        200:
          description: OK
      tags:
      - Outcomes
      - Id
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