swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/object/setObjectDoNotRegisterFlag:
    post:
      summary: Switch Apply Flag
      description: '* DO NOT USE. This API will be deleted.<br>Switch the Apply flag
        on or off.'
      operationId: config
      x-api-path-slug: v1objectsetobjectdonotregisterflag-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Switch
      - Apply
      - Flag
  /v1/object/setGroupDoNotRegisterFlag:
    post:
      summary: Switch Apply Flag per Group
      description: '* DO NOT USE. This API will be deleted.<br>Switch the Apply flag
        per group'
      operationId: groupConfig
      x-api-path-slug: v1objectsetgroupdonotregisterflag-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Switch
      - Apply
      - Flag
      - Per
      - Group