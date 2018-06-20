---
swagger: "2.0"
x-collection-name: TidyHQ
x-complete: 0
info:
  title: API Evangelist Building Block API Get Tools for Building Block
  description: retrieve building block tools
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
  /buildingblocks/bytype/{type}:
    get:
      summary: Get Building Blocks by Type
      description: building blocks by type
      operationId: getBuildingBlocksByType
      x-api-path-slug: buildingblocksbytypetype-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: type
        description: the building block type to filter by
      responses:
        200:
          description: OK
      tags:
      - Building
      - Blocks
      - By
      - Type
  /buildingblocks/categories/:
    get:
      summary: Get Categories for Building Block
      description: retrieve building block categories
      operationId: getBuildingBlockCategories
      x-api-path-slug: buildingblockscategories-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      responses:
        200:
          description: OK
      tags:
      - CategoriesBuilding
      - Block
    post:
      summary: Add Category for Building Block
      description: add building block category
      operationId: addBuildingBlockCategory
      x-api-path-slug: buildingblockscategories-post
      parameters:
      - in: formData
        name: appid
        description: your appid for accessing the building block
      - in: formData
        name: appkey
        description: your appkey for accessing the building block
      - in: formData
        name: name
        description: a name for the url
      - in: formData
        name: type
        description: type of url
      - in: formData
        name: url
        description: the url
      responses:
        200:
          description: OK
      tags:
      - CategoryBuilding
      - Block
  /buildingblocks/categories/{category_id}:
    delete:
      summary: Delete Category for Building Block
      description: delete a building block category
      operationId: deleteBuildingBlockCategory
      x-api-path-slug: buildingblockscategoriescategory-id-delete
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: category_id
        description: id for the building block
      responses:
        200:
          description: OK
      tags:
      - CategoryBuilding
      - Block
  /buildingblocks/{building_block_id}/:
    delete:
      summary: Delete Building Block
      description: delete building block
      operationId: deleteBuildingBlock
      x-api-path-slug: buildingblocksbuilding-block-id-delete
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: the unique id for buildingblock entry
      responses:
        200:
          description: OK
      tags:
      - Building
      - Block
    get:
      summary: Get Building Block
      description: Returns the building block detail
      operationId: getBuildingBlock
      x-api-path-slug: buildingblocksbuilding-block-id-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: the unique id for buildingblock entry
      responses:
        200:
          description: OK
      tags:
      - Building
      - Block
    put:
      summary: Update Building Block
      description: update building block
      operationId: updateBuildingBlock
      x-api-path-slug: buildingblocksbuilding-block-id-put
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
      - in: path
        name: building_block_id
        description: the unique id for buildingblock entry
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
  /buildingblocks/{building_block_id}/images/:
    get:
      summary: Get Images for Building Block
      description: get building block images
      operationId: getBuildingBlockImages
      x-api-path-slug: buildingblocksbuilding-block-idimages-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for building block
      responses:
        200:
          description: OK
      tags:
      - ImagesBuilding
      - Block
    post:
      summary: Add Image for Building Block
      description: add building block image
      operationId: addBuildingBlockImage
      x-api-path-slug: buildingblocksbuilding-block-idimages-post
      parameters:
      - in: formData
        name: appid
        description: your appid for accessing the building block
      - in: formData
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for the building block
      - in: formData
        name: name
        description: image name
      - in: formData
        name: path
        description: image path
      - in: formData
        name: type
        description: image type
      responses:
        200:
          description: OK
      tags:
      - ImageBuilding
      - Block
  /buildingblocks/{building_block_id}/images/{image_id}:
    delete:
      summary: Delete Image for Building Block
      description: delete a building block image
      operationId: deleteBuildingBlockImage
      x-api-path-slug: buildingblocksbuilding-block-idimagesimage-id-delete
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for the building block
      - in: path
        name: image_id
        description: id for the image to remove from building block
      responses:
        200:
          description: OK
      tags:
      - ImageBuilding
      - Block
  /buildingblocks/{building_block_id}/logs/:
    get:
      summary: Get Logs for Building Block
      description: get building block logs
      operationId: getBuildingBlockLogs
      x-api-path-slug: buildingblocksbuilding-block-idlogs-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for building block
      responses:
        200:
          description: OK
      tags:
      - LogsBuilding
      - Block
    post:
      summary: Add Log for Building Block
      description: add building block log
      operationId: addBuildingBlockLog
      x-api-path-slug: buildingblocksbuilding-block-idlogs-post
      parameters:
      - in: formData
        name: appid
        description: your appid for accessing the building block
      - in: formData
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for the building block
      - in: formData
        name: details
        description: log details
      - in: formData
        name: type
        description: type of log entry
      responses:
        200:
          description: OK
      tags:
      - LogBuilding
      - Block
  /buildingblocks/{building_block_id}/logs/{log_id}:
    delete:
      summary: Delete Log for Building Block
      description: delete a building block log
      operationId: deleteBuildingBlockLog
      x-api-path-slug: buildingblocksbuilding-block-idlogslog-id-delete
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for the building block
      - in: path
        name: log_id
        description: id for the log
      responses:
        200:
          description: OK
      tags:
      - LogBuilding
      - Block
  /buildingblocks/{building_block_id}/organization/:
    get:
      summary: Get Organizations for Building Block
      description: retrieve building block companies
      operationId: getBuildingBlockOrganizations
      x-api-path-slug: buildingblocksbuilding-block-idorganization-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for building block
      responses:
        200:
          description: OK
      tags:
      - OrganizationsBuilding
      - Block
    post:
      summary: Add Organization for Building Block
      description: add organization to building block
      operationId: addBuildingBlockOrganization
      x-api-path-slug: buildingblocksbuilding-block-idorganization-post
      parameters:
      - in: formData
        name: appid
        description: your appid for accessing the building block
      - in: formData
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for the building block
      - in: formData
        name: organization_id
        description: the unique organization id
      - in: formData
        name: url
        description: url for the tool
      responses:
        200:
          description: OK
      tags:
      - OrganizationBuilding
      - Block
  /buildingblocks/{building_block_id}/organization/{organization_id}:
    delete:
      summary: Delete Organization for Building Block
      description: delete a building block organization
      operationId: getBuildingBlockOrganization
      x-api-path-slug: buildingblocksbuilding-block-idorganizationorganization-id-delete
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for the building block
      - in: path
        name: organization_id
        description: organization to remove from building block
      responses:
        200:
          description: OK
      tags:
      - OrganizationBuilding
      - Block
  /buildingblocks/{building_block_id}/tags/:
    get:
      summary: Get Tags for Building Block
      description: building block tags
      operationId: getbuildingblockTags
      x-api-path-slug: buildingblocksbuilding-block-idtags-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for building block
      responses:
        200:
          description: OK
      tags:
      - TagsBuilding
      - Block
    post:
      summary: Add Tag for Building Block
      description: add tag to building block
      operationId: addBuildingBlockTag
      x-api-path-slug: buildingblocksbuilding-block-idtags-post
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for the building block
      - in: query
        name: tag
        description: tag name
      responses:
        200:
          description: OK
      tags:
      - TagBuilding
      - Block
  /buildingblocks/{building_block_id}/tags/{tag}:
    delete:
      summary: Delete Tag for Building Block
      description: delete buildingblock tag
      operationId: deletebuildingblockTag
      x-api-path-slug: buildingblocksbuilding-block-idtagstag-delete
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for the building block
      - in: path
        name: tag
        description: tag to remove from building block
      responses:
        200:
          description: OK
      tags:
      - TagBuilding
      - Block
  /buildingblocks/{building_block_id}/tools/:
    get:
      summary: Get Tools for Building Block
      description: retrieve building block tools
      operationId: getBuildingBlockTools
      x-api-path-slug: buildingblocksbuilding-block-idtools-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      - in: path
        name: building_block_id
        description: id for building block
      responses:
        200:
          description: OK
      tags:
      - ToolsBuilding
      - Block
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