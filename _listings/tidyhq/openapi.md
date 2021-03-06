---
swagger: "2.0"
x-collection-name: TidyHQ
x-complete: 1
info:
  title: API Evangelist Tools API
  description: this-is-an-api-that-provides-access-to-the-tools-that-i-curate-from-around-the-api-space-
  termsOfService: http://developer.apievangelist.com/index.html
  contact:
    name: Kin Lane
    url: http://kinlane.com
    email: info@apievangelist.com
  license:
    name: MIT
    url: http://opensource.org/licenses/MIT
  version: "1.0"
host: api.apievangelist.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tool/{id}:
    get:
      summary: Retrieve a tool using its ID
      description: Returns a tool detail
      operationId: getTool
      x-api-path-slug: toolid-get
      parameters:
      - in: query
        name: appid
        description: application id for application making calls
      - in: query
        name: appkey
        description: application key for application making calls
      - in: path
        name: id
        description: id of the tool to be returned
      responses:
        200:
          description: Successful Analysis Response
      tags:
      - ""
  /tools/:
    get:
      summary: Pull tool
      description: Returns a list of all tools filtered by keyword.
      operationId: getTool
      x-api-path-slug: tools-get
      parameters:
      - in: query
        name: appid
        description: application id for application making calls
      - in: query
        name: appkey
        description: application key for application making calls
      - in: query
        name: query
        description: a text query to search across tools
      responses:
        200:
          description: Successful Analysis Response
      tags:
      - ""
---