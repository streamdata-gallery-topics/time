---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Post Projects Issues Issue Time Estimate
  version: 1.0.0
  description: Post projects issues issue time estimate.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/issues/{issue_id}/time_estimate:
    post:
      summary: Post Projects Issues Issue Time Estimate
      description: Post projects issues issue time estimate.
      operationId: postV3ProjectsIdIssuesIssueIdTimeEstimate
      x-api-path-slug: v3projectsidissuesissue-idtime-estimate-post
      parameters:
      - in: formData
        name: duration
        description: The duration to be parsed
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Time
      - Estimate
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