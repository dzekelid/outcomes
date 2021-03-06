---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Create/link an outcome
  description: Create/link an outcome.
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
  /courses/{course_id}/outcome_groups/id/outcomes:
    get:
      summary: List linked outcomes
      description: List linked outcomes.
      operationId: list-linked-outcomes
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomes-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Outcomes
    post:
      summary: Create/link an outcome
      description: Create/link an outcome.
      operationId: createlink-an-outcome
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomes-post
      parameters:
      - in: query
        name: calculation_int
        description: The new calculation int
      - in: query
        name: calculation_method
        description: The new calculation method
      - in: query
        name: description
        description: The description of the new outcome
      - in: query
        name: display_name
        description: A friendly name shown in reports for outcomes with cryptic titles,
          such asncommon core standards names
      - in: query
        name: mastery_points
        description: The mastery threshold for the embedded rubric criterion
      - in: query
        name: outcome_id
        description: The ID of the existing outcome to link
      - in: query
        name: ratings[][description]
        description: The description of a rating level for the embedded rubric criterion
      - in: query
        name: ratings[][points]
        description: The points corresponding to a rating level for the embedded rubricncriterion
      - in: query
        name: title
        description: The title of the new outcome
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Outcomes
  /courses/{course_id}/outcome_groups/id/outcomes/{outcome_id}:
    delete:
      summary: Unlink an outcome
      description: Unlink an outcome.
      operationId: unlink-an-outcome
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomesoutcome-id-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Outcomes
      - Outcome
      - Id
    put:
      summary: Create/link an outcome
      description: Create/link an outcome.
      operationId: createlink-an-outcome
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomesoutcome-id-put
      parameters:
      - in: query
        name: calculation_int
        description: The new calculation int
      - in: query
        name: calculation_method
        description: The new calculation method
      - in: query
        name: description
        description: The description of the new outcome
      - in: query
        name: display_name
        description: A friendly name shown in reports for outcomes with cryptic titles,
          such asncommon core standards names
      - in: query
        name: mastery_points
        description: The mastery threshold for the embedded rubric criterion
      - in: query
        name: outcome_id
        description: The ID of the existing outcome to link
      - in: query
        name: ratings[][description]
        description: The description of a rating level for the embedded rubric criterion
      - in: query
        name: ratings[][points]
        description: The points corresponding to a rating level for the embedded rubricncriterion
      - in: query
        name: title
        description: The title of the new outcome
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Outcomes
      - Outcome
      - Id
  /courses/{course_id}/outcome_groups:
    get:
      summary: Get all outcome groups for context
      description: Get all outcome groups for context.
      operationId: get-all-outcome-groups-for-context
      x-api-path-slug: coursescourse-idoutcome-groups-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
  /courses/{course_id}/outcome_groups/id:
    delete:
      summary: Delete an outcome group
      description: Delete an outcome group.
      operationId: delete-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
    get:
      summary: Show an outcome group
      description: Show an outcome group.
      operationId: show-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
    put:
      summary: Update an outcome group
      description: Update an outcome group.
      operationId: update-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsid-put
      parameters:
      - in: query
        name: description
        description: The new outcome group description
      - in: query
        name: parent_outcome_group_id
        description: The id of the new parent outcome group
      - in: query
        name: title
        description: The new outcome group title
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
  /courses/{course_id}/outcome_groups/id/import:
    post:
      summary: Import an outcome group
      description: Import an outcome group.
      operationId: import-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsidimport-post
      parameters:
      - in: query
        name: source_outcome_group_id
        description: The ID of the source outcome group
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Import
  /courses/{course_id}/outcome_groups/id/subgroups:
    get:
      summary: List subgroups
      description: List subgroups.
      operationId: list-subgroups
      x-api-path-slug: coursescourse-idoutcome-groupsidsubgroups-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Subgroups
    post:
      summary: Create a subgroup
      description: Create a subgroup.
      operationId: create-a-subgroup
      x-api-path-slug: coursescourse-idoutcome-groupsidsubgroups-post
      parameters:
      - in: query
        name: description
        description: The description of the new outcome group
      - in: query
        name: title
        description: The title of the new outcome group
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Subgroups
  /courses/{course_id}/outcome_group_links:
    get:
      summary: Get all outcome links for context
      description: Get all outcome links for context.
      operationId: get-all-outcome-links-for-context
      x-api-path-slug: coursescourse-idoutcome-group-links-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Group
      - Links
  /courses/{course_id}/outcome_results:
    get:
      summary: Get outcome results
      description: Get outcome results.
      operationId: get-outcome-results
      x-api-path-slug: coursescourse-idoutcome-results-get
      parameters:
      - in: query
        name: include[]
        description: String, u201calignmentsu201d|u201coutcomesu201d|u201coutcomes
      - in: query
        name: outcome_ids[]
        description: If specified, only the outcomes whose ids are given will be included
          in thenresults
      - in: query
        name: user_ids[]
        description: If specified, only the users whose ids are given will be included
          in thenresults
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Results
  /courses/{course_id}/outcome_rollups:
    get:
      summary: Get outcome result rollups
      description: Get outcome result rollups.
      operationId: get-outcome-result-rollups
      x-api-path-slug: coursescourse-idoutcome-rollups-get
      parameters:
      - in: query
        name: aggregate
        description: If specified, instead of returning one rollup for each user,
          all the usernrollups will be combined into one rollup for the course that
          will containnthe average rollup score for each outcome
      - in: query
        name: include[]
        description: String, u201ccoursesu201d|u201coutcomesu201d|u201coutcomes
      - in: query
        name: outcome_ids[]
        description: If specified, only the outcomes whose ids are given will be included
          in thenresults
      - in: query
        name: user_ids[]
        description: If specified, only the users whose ids are given will be included
          in thenresults or used in an aggregate result
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Rollups
  /courses/{course_id}/root_outcome_group:
    get:
      summary: Redirect to root outcome group for context
      description: Redirect to root outcome group for context.
      operationId: redirect-to-root-outcome-group-for-context
      x-api-path-slug: coursescourse-idroot-outcome-group-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Root
      - Outcome
      - Group
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