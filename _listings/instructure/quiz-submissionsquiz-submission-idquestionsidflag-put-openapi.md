---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Quiz Submissions API Flagging a question.
  description: Flagging a question..
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
  /quiz_submissions/{quiz_submission_id}/questions/id/flag:
    put:
      summary: Flagging a question.
      description: Flagging a question..
      operationId: flagging-a-question
      x-api-path-slug: quiz-submissionsquiz-submission-idquestionsidflag-put
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: attempt
        description: The attempt number of the quiz submission being taken
      - in: query
        name: validation_token
        description: The unique validation token you received when the Quiz Submission
          wasncreated
      responses:
        200:
          description: OK
      tags:
      - Quiz
      - Submissions
      - Quiz
      - Submission
      - Id
      - Questions
      - Id
      - Flag
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