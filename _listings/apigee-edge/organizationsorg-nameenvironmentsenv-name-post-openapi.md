---
swagger: "2.0"
x-collection-name: Apigee Edge
x-complete: 0
info:
  title: Apigee Edge Post Organizations Name Environments Env Name
  description: Updates an environment.
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{org_name}/environments:
    get:
      summary: Get Organizations Name Environments
      description: Lists all the environments in an organization.
      operationId: getOrganizationsOrgNameEnvironments
      x-api-path-slug: organizationsorg-nameenvironments-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
    post:
      summary: Post Organizations Name Environments
      description: Creates an environment.
      operationId: postOrganizationsOrgNameEnvironments
      x-api-path-slug: organizationsorg-nameenvironments-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
  /organizations/{org_name}/environments/{env_name}:
    get:
      summary: Get Organizations Name Environments Env Name
      description: Gets details for an environment.
      operationId: getOrganizationsOrgNameEnvironmentsEnvName
      x-api-path-slug: organizationsorg-nameenvironmentsenv-name-get
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
    post:
      summary: Post Organizations Name Environments Env Name
      description: Updates an environment.
      operationId: postOrganizationsOrgNameEnvironmentsEnvName
      x-api-path-slug: organizationsorg-nameenvironmentsenv-name-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
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