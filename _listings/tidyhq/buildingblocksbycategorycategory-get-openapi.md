---
swagger: "2.0"
x-collection-name: TidyHQ
x-complete: 0
info:
  title: API Evangelist Building Block API Get Building Blocks by Category
  description: building blocks by category
  contact:
    name: Kin Lane
    url: http://kinlane.com
    email: info@kinlane.com
  version: v1
host: buildingblock.api.kinlane.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /buildingblocks/:
    get:
      summary: Get All Building Blocks
      description: all building blocks
      operationId: getBuildingBlocks
      x-api-path-slug: buildingblocks-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: query
        name: count
        description: how many to show on page
      - in: query
        name: page
        description: which page of results to show
      - in: query
        name: query
        description: a text query to search across building block
      - in: query
        name: sort
        description: which field to sort by
      responses:
        200:
          description: OK
      tags:
      - Building
      - Blocks
    post:
      summary: Add Building Block
      description: add a building block post
      operationId: addBuildingBlock
      x-api-path-slug: buildingblocks-post
      parameters:
      - in: query
        name: about
        description: details about the building block
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: query
        name: building_block_category_id
        description: the category for the building block
      - in: query
        name: name
        description: name of the building block
      - in: query
        name: sort_order
        description: sort_order for the building block
      responses:
        200:
          description: OK
      tags:
      - Building
      - Block
  /buildingblocks/bycategory/{category}:
    get:
      summary: Get Building Blocks by Category
      description: building blocks by category
      operationId: getBuildingBlocksByCategory
      x-api-path-slug: buildingblocksbycategorycategory-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: category
        description: the building block category to filter by
      responses:
        200:
          description: OK
      tags:
      - Building
      - Blocks
      - By
      - Category
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