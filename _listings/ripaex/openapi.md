---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 1
info:
  title: RIPA Node Documentation
  description: this-is-a-documentation-for-ripanodehttpsgithub-comripaexripanode-built-with-swagger-ui-to-make-testing-a-breeze--if-you-find-any-issues-come-over-to-ripaexripanodetestapihttpsgithub-comripaexripanodetestapi-to-open-an-issue-or-even-better-send-a-pr-that-fixes-the-issue-the-community-ssl-public-api-used-as-test-host-is-provided-from-ripaex-iohttpswww-ripaex-io-
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/loader/autoconfigure:
    get:
      summary: Loader Autoconfigure
      description: Auto-configure the client loader.
      operationId: loader.autoconfigure
      x-api-path-slug: apiloaderautoconfigure-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Loader
      - Autoconfigure
  /api/loader/status:
    get:
      summary: Loader Status
      description: Get the blockchain status.
      operationId: loader.status
      x-api-path-slug: apiloaderstatus-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Loader
      - Status
  /api/loader/status/sync:
    get:
      summary: Loader Status Sync
      description: Get the synchronisation status of the client.
      operationId: loader.sync
      x-api-path-slug: apiloaderstatussync-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Loader
      - Status
      - Sync
---