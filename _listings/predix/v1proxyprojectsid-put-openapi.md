---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix SAS ESP Predix Service Load/Create Project
  description: API to Load/Create project in ESP server.
  contact:
    name: zahid.iqbal2@ge.com
  version: 1.0.0
host: sas-proxy.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/catalog/taxonomy:
    post:
      summary: Load a taxonomy.
      description: This operation loads the supplied taxonomy structure into catalog.
        If a taxonomy already exists in the catalog, new paths in the supplied structure
        will be added. It will not delete existing paths.
      operationId: loadTaxonomy
      x-api-path-slug: apiv1catalogtaxonomy-post
      parameters:
      - in: body
        name: body
        description: taxonomy JSON request
        schema:
          $ref: '#/definitions/holder'
      responses:
        2:
          description: Successful response
      tags:
      - Load
      - Taxonomy
  /v1/proxy/projects/{id}:
    put:
      summary: Load/Create Project
      description: API to Load/Create project in ESP server.
      operationId: loadOrCreateProjectUsingPUT
      x-api-path-slug: v1proxyprojectsid-put
      parameters:
      - in: body
        name: reqBody
        description: reqBody
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Load
      - Project
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