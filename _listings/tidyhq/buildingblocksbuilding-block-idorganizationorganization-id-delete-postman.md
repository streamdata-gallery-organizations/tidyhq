{
  "info": {
    "name": "API Evangelist Building Block API Delete Organization for Building Block",
    "_postman_id": "a3e6a336-ca56-4370-bbb7-5f7af398c57c",
    "description": "delete a building block organization",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Building",
      "item": [
        {
          "id": "c679a55f-8e3a-4dc9-b9f4-a4401b15cf69",
          "name": "getBuildingBlocks",
          "request": {
            "url": "http://buildingblock.api.kinlane.com/buildingblocks/?appid=%7B%7D&appkey=%7B%7D&count=%7B%7D&page=%7B%7D&query=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "all building blocks"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2860c192-5da4-495c-9fa9-d2ff1f2ee628"
            }
          ]
        },
        {
          "id": "22ce89b3-67ea-4d9f-bd7c-cb93b3f960d7",
          "name": "addBuildingBlock",
          "request": {
            "url": "http://buildingblock.api.kinlane.com/buildingblocks/?about=%7B%7D&appid=%7B%7D&appkey=%7B%7D&building_block_category_id=%7B%7D&name=%7B%7D&sort_order=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "add a building block post"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3098a8c-2aae-496c-8119-529b06dd0bcf"
            }
          ]
        },
        {
          "id": "0bfe678e-c2c7-4073-8e2e-f9c672769d25",
          "name": "getBuildingBlocksByCategory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/bycategory/:category"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "category",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "building blocks by category"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d816114e-0da9-464d-b909-e37bbab36715"
            }
          ]
        },
        {
          "id": "3d541887-6042-4529-8659-ee08df1db24f",
          "name": "getBuildingBlocksByType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/bytype/:type"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "building blocks by type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c659d7d2-6708-4045-9573-020fe0e80882"
            }
          ]
        },
        {
          "id": "bdee346e-30da-4633-8fff-7a937888e787",
          "name": "getBuildingBlock",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the building block detail"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47572bb8-4726-4c7d-8171-420e293863c7"
            }
          ]
        },
        {
          "id": "768aa8a9-aedf-4526-a994-4ec629031b7e",
          "name": "updateBuildingBlock",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/"
              ],
              "query": [
                {
                  "key": "about",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "building_block_category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_order",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "update building block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5642179-cb1e-4690-8bdf-7bc3b395a6f9"
            }
          ]
        },
        {
          "id": "8f58e093-5be1-4f16-863e-93b9670431bc",
          "name": "deleteBuildingBlock",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "delete building block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdde892f-b9a0-49a8-bc6e-f19ad4533793"
            }
          ]
        }
      ]
    },
    {
      "name": "CategoriesBuilding",
      "item": [
        {
          "id": "048834ff-506e-4dda-87d7-7254a8c1f0b2",
          "name": "getBuildingBlockCategories",
          "request": {
            "url": "http://buildingblock.api.kinlane.com/buildingblocks/categories/?appid=%7B%7D&appkey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "retrieve building block categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4245cb02-1b86-4ab9-9f57-800c8c600f1e"
            }
          ]
        }
      ]
    },
    {
      "name": "CategoryBuilding",
      "item": [
        {
          "id": "0b303834-2522-4e4e-b3e0-28e75f0d4596",
          "name": "addBuildingBlockCategory",
          "request": {
            "url": "http://buildingblock.api.kinlane.com/buildingblocks/categories/",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "appid",
                  "value": "{}",
                  "disabled": false,
                  "description": "your appid for accessing the building block"
                },
                {
                  "key": "appkey",
                  "value": "{}",
                  "disabled": false,
                  "description": "your appkey for accessing the building block"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "a name for the url"
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": "type of url"
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": "the url"
                }
              ]
            },
            "description": "add building block category"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2b12222-0a71-4d63-a41e-70e1f981d056"
            }
          ]
        },
        {
          "id": "028e231b-6029-447c-ae0c-851898ef7ee1",
          "name": "deleteBuildingBlockCategory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/categories/:category_id"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "category_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "delete a building block category"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66aef3db-845e-4f67-99b6-3bf744bfd30a"
            }
          ]
        }
      ]
    },
    {
      "name": "ImagesBuilding",
      "item": [
        {
          "id": "677b7027-ff79-4d10-8d8c-0c8076dad3d3",
          "name": "getBuildingBlockImages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/images/"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "get building block images"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d30d89b4-c915-40cb-80de-ee64b60d96ea"
            }
          ]
        }
      ]
    },
    {
      "name": "ImageBuilding",
      "item": [
        {
          "id": "9596070f-bf44-4ca3-8d72-8dd9bfc5d009",
          "name": "addBuildingBlockImage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/images/"
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "appid",
                  "value": "{}",
                  "disabled": false,
                  "description": "your appid for accessing the building block"
                },
                {
                  "key": "appkey",
                  "value": "{}",
                  "disabled": false,
                  "description": "your appkey for accessing the building block"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "image name"
                },
                {
                  "key": "path",
                  "value": "{}",
                  "disabled": false,
                  "description": "image path"
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": "image type"
                }
              ]
            },
            "description": "add building block image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc4b2fa1-6c7e-409d-8943-4938705381d9"
            }
          ]
        },
        {
          "id": "efeb0dfa-b29a-4889-8880-edf1c7e8db07",
          "name": "deleteBuildingBlockImage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/images/:image_id"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "image_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "delete a building block image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cab8dbb9-180a-4dea-9ef3-a25a66390fa0"
            }
          ]
        }
      ]
    },
    {
      "name": "LogsBuilding",
      "item": [
        {
          "id": "7ec1687e-91cc-411b-b2f9-cda5a408da03",
          "name": "getBuildingBlockLogs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/logs/"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "get building block logs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d90b4931-c6f1-40a0-98b8-1a07325c95eb"
            }
          ]
        }
      ]
    },
    {
      "name": "LogBuilding",
      "item": [
        {
          "id": "edff6482-9974-49a4-9e22-d7baa74e0b75",
          "name": "addBuildingBlockLog",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/logs/"
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "appid",
                  "value": "{}",
                  "disabled": false,
                  "description": "your appid for accessing the building block"
                },
                {
                  "key": "appkey",
                  "value": "{}",
                  "disabled": false,
                  "description": "your appkey for accessing the building block"
                },
                {
                  "key": "details",
                  "value": "{}",
                  "disabled": false,
                  "description": "log details"
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": "type of log entry"
                }
              ]
            },
            "description": "add building block log"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b920576-3683-4d78-8726-a3a7a55132f9"
            }
          ]
        },
        {
          "id": "989bc9af-3139-4631-ad3a-50fcb6f01f90",
          "name": "deleteBuildingBlockLog",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/logs/:log_id"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "log_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "delete a building block log"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2343784-2371-40f1-af4b-17f7e9fc50d1"
            }
          ]
        }
      ]
    },
    {
      "name": "OrganizationsBuilding",
      "item": [
        {
          "id": "6c8c1e42-7108-479d-b2ad-8d2c66fbcf2d",
          "name": "getBuildingBlockOrganizations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/organization/"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "retrieve building block companies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf8ab09a-1605-4608-b113-081ace624498"
            }
          ]
        }
      ]
    },
    {
      "name": "OrganizationBuilding",
      "item": [
        {
          "id": "9eb17ecb-416c-487c-a693-6fbdb8493ca7",
          "name": "addBuildingBlockOrganization",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/organization/"
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "appid",
                  "value": "{}",
                  "disabled": false,
                  "description": "your appid for accessing the building block"
                },
                {
                  "key": "appkey",
                  "value": "{}",
                  "disabled": false,
                  "description": "your appkey for accessing the building block"
                },
                {
                  "key": "organization_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "the unique organization id"
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": "url for the tool"
                }
              ]
            },
            "description": "add organization to building block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "485c2912-6f15-47d4-b9ef-224a39819898"
            }
          ]
        },
        {
          "id": "c782897a-f663-477b-b424-faa9cdea91f7",
          "name": "getBuildingBlockOrganization",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/organization/:organization_id"
              ],
              "query": [
                {
                  "key": "appid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appkey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "building_block_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "organization_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "delete a building block organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f5cc713-76e3-4721-ba34-1fbb7a14d1e8"
            }
          ]
        }
      ]
    }
  ]
}