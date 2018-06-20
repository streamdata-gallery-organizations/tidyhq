{
  "info": {
    "name": "API Evangelist Building Block API Add Tool for Building Block",
    "_postman_id": "25c90851-6e16-497d-922b-85264f700008",
    "description": "add tool to building block",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Building",
      "item": [
        {
          "id": "4957389a-100b-4130-b4fb-2078e160e176",
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
              "id": "09165cab-d4d8-4560-9c89-c9d34857b11b"
            }
          ]
        },
        {
          "id": "f1346675-95b1-4cc7-9f7c-eb6b9be31b16",
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
              "id": "5d0818d6-5968-4ab0-a571-d22ea6f9f9bb"
            }
          ]
        },
        {
          "id": "e8dd6ab2-e277-4630-a9b4-5b5a52626fd2",
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
              "id": "560cf5c3-f8a0-4ac8-bd2e-7faa713ea45a"
            }
          ]
        },
        {
          "id": "80fa98d3-4ba1-4b96-ba58-7d4ade319d13",
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
              "id": "8f77e0ec-ea8d-4391-a8f7-bf2e2e39c2cb"
            }
          ]
        },
        {
          "id": "2714fd8d-4da9-44b6-ab25-457ff656cedf",
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
              "id": "1ed70a3f-4b3c-44da-beb4-dd29a4e86ecf"
            }
          ]
        },
        {
          "id": "e11d14d0-22a1-47b3-926b-15c7935b3173",
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
              "id": "6c554beb-1196-42ca-bd24-8cb7d8727c8f"
            }
          ]
        },
        {
          "id": "3181dd8a-6cdf-4940-af68-8e4609a510a5",
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
              "id": "94478647-aa6a-4d88-86d3-e4aa627e954b"
            }
          ]
        }
      ]
    },
    {
      "name": "CategoriesBuilding",
      "item": [
        {
          "id": "5148a901-5138-4b12-9f4f-9dd4e2114456",
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
              "id": "3d9be0d3-4b7a-4d7d-8395-136be3fb8cbf"
            }
          ]
        }
      ]
    },
    {
      "name": "CategoryBuilding",
      "item": [
        {
          "id": "5e40050c-0949-4d86-b5bd-02a1cb73f1b5",
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
              "id": "e14cebec-128a-43e4-95e1-b0a302ae05f2"
            }
          ]
        },
        {
          "id": "1cd67235-cc8d-4daf-91fb-9d9477f037fb",
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
              "id": "46781f6c-925e-4cda-af6f-22a8a835feae"
            }
          ]
        }
      ]
    },
    {
      "name": "ImagesBuilding",
      "item": [
        {
          "id": "ac36c740-6475-4644-b10d-fe503614f723",
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
              "id": "c5515542-4db8-48a7-a546-b232032e4fe9"
            }
          ]
        }
      ]
    },
    {
      "name": "ImageBuilding",
      "item": [
        {
          "id": "bd2d062c-490f-4ab8-ab5f-254c0af511ea",
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
              "id": "decfd17b-50db-48a0-bb8b-5616719bab0a"
            }
          ]
        },
        {
          "id": "2b2b8368-9ac5-422c-ba1a-b0ab236f37aa",
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
              "id": "9147d57a-e38d-4497-8c46-b9c908119d5c"
            }
          ]
        }
      ]
    },
    {
      "name": "LogsBuilding",
      "item": [
        {
          "id": "5d724c46-2cdf-43c6-8f2c-29df1bf03f08",
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
              "id": "8e7a3c5b-93e3-437f-93e4-0c88391628ff"
            }
          ]
        }
      ]
    },
    {
      "name": "LogBuilding",
      "item": [
        {
          "id": "4c3c2f0e-6be6-4dcf-94ff-fe12b673f7e5",
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
              "id": "7c46a171-2e08-4077-b5db-a56a1a65f399"
            }
          ]
        },
        {
          "id": "631c4816-f11a-4d3b-8531-294570af86ed",
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
              "id": "3385628d-1ea3-47a1-8057-d764e587be40"
            }
          ]
        }
      ]
    },
    {
      "name": "OrganizationsBuilding",
      "item": [
        {
          "id": "11a32b69-0b2b-4550-b03e-a46341b3cf4f",
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
              "id": "df2b0975-bcc6-468b-8148-cb9349d10002"
            }
          ]
        }
      ]
    },
    {
      "name": "OrganizationBuilding",
      "item": [
        {
          "id": "9b4a4870-6e0d-4b4c-96d4-08964ec3ab3c",
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
              "id": "4117ff2b-9996-469c-8040-152b16634b2a"
            }
          ]
        },
        {
          "id": "6a1e60ae-678e-47f0-96eb-ad0458ce458c",
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
              "id": "a063d7b0-9142-4659-8e0e-12f666494f08"
            }
          ]
        }
      ]
    },
    {
      "name": "TagsBuilding",
      "item": [
        {
          "id": "5d1c88a3-a9bb-4ef4-82b7-35065661518c",
          "name": "getbuildingblockTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/tags/"
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
            "description": "building block tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19727152-1c04-4ef8-b6d8-d3f50c157f95"
            }
          ]
        }
      ]
    },
    {
      "name": "TagBuilding",
      "item": [
        {
          "id": "42df3189-44a7-4e9c-a925-55516561cfe5",
          "name": "addBuildingBlockTag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/tags/"
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
                },
                {
                  "key": "tag",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "add tag to building block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27b432b0-c56b-4da6-a34d-7506d69fdd14"
            }
          ]
        },
        {
          "id": "c1a4bfac-908a-49ce-9c65-c648de50bc98",
          "name": "deletebuildingblockTag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/tags/:tag"
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
                  "id": "tag",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "delete buildingblock tag"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "886af817-3e1a-4d15-b621-7631606b3dd1"
            }
          ]
        }
      ]
    },
    {
      "name": "ToolsBuilding",
      "item": [
        {
          "id": "84be511b-9578-4cc1-8427-69b19fe4f2b8",
          "name": "getBuildingBlockTools",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/tools/"
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
            "description": "retrieve building block tools"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1fabfb2-baf3-459a-bc6c-880b490a188d"
            }
          ]
        }
      ]
    },
    {
      "name": "ToolBuilding",
      "item": [
        {
          "id": "e33787b1-d2b4-4565-bc9d-9e494a15710d",
          "name": "addBuildingBlockTool",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/tools/"
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
                  "key": "tool_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "the unique tool id"
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": "url for the tool"
                }
              ]
            },
            "description": "add tool to building block"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0c8ae03-fc1d-41c4-90c0-d176a7374d06"
            }
          ]
        }
      ]
    }
  ]
}