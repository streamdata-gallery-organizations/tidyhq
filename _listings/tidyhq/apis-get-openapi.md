---
swagger: "2.0"
x-collection-name: TidyHQ
x-complete: 0
info:
  title: API Evangelist API API Retrieve APIs
  description: Returns a list of APIs.
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
  /api/{id}:
    get:
      summary: Retrieve an API
      description: Returns the API detail
      operationId: getAPI
      x-api-path-slug: apiid-get
      parameters:
      - in: query
        name: appid
        description: application id for application making calls
      - in: query
        name: appkey
        description: application key for application making calls
      - in: path
        name: id
        description: id of the blog post to be returned
      responses:
        200:
          description: Successful Image Manipulation
          schema:
            type: array
            items:
              $ref: '#/definitions/Image'
      tags:
      - APIs
      - Discovery
  /apis:
    get:
      summary: Retrieve APIs
      description: Returns a list of APIs.
      operationId: getAPI
      x-api-path-slug: apis-get
      parameters:
      - in: query
        name: appid
        description: application id for application making calls
      - in: query
        name: appkey
        description: application key for application making calls
      - in: query
        name: date
        description: data to search by in the m/d/Y format
      - in: query
        name: limit
        description: how many posts to show
      - in: query
        name: new
        description: only show new apis (true / false)
      - in: query
        name: query
        description: a text query to search across posts
      responses:
        200:
          description: Successful Image Manipulation
          schema:
            type: array
            items:
              $ref: '#/definitions/Image'
      tags:
      - APIs
      - Discovery
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