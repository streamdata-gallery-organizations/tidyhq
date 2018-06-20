{
  "info": {
    "name": "API Evangelist Building Block API Get URLs for Building Block",
    "_postman_id": "62a19802-ecee-4c85-9fe8-85ff577c8a22",
    "description": "retrieve building block url",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Building",
      "item": [
        {
          "id": "bda117a1-1b80-4cd8-bbb1-e2cbc6b98055",
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
              "id": "90856c11-5811-4dea-a4d0-3a5ae1a03d78"
            }
          ]
        },
        {
          "id": "edc3d273-828e-407f-b444-c941f4cd1c3a",
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
              "id": "a27d33ca-42f0-47da-bfe4-f23c449ff1e6"
            }
          ]
        },
        {
          "id": "c9b151a6-dc4c-4ea4-b68d-3a62f85bb5fd",
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
              "id": "1aeb6612-c6b7-4214-9f8d-f44f749bf099"
            }
          ]
        },
        {
          "id": "3c08b58f-514f-4a08-82f2-aee4fc89ba45",
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
              "id": "d622cf24-b7f7-4e35-80b2-d9e1e32b8875"
            }
          ]
        },
        {
          "id": "ea0c88ed-2170-4373-9914-ba29f5bc31ad",
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
              "id": "d597ebb1-1fad-405e-aef7-1b73eb80c045"
            }
          ]
        },
        {
          "id": "8e6accd6-0323-4a77-803e-b846fda95da6",
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
              "id": "287ee988-4e11-4943-9b4d-88f742cb3076"
            }
          ]
        },
        {
          "id": "b95926c6-4bb7-458e-b4e2-c8058a8967da",
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
              "id": "b956b715-135c-4f1d-b939-069b5318be1d"
            }
          ]
        }
      ]
    },
    {
      "name": "CategoriesBuilding",
      "item": [
        {
          "id": "663add08-6ece-431b-adca-2a45d8312222",
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
              "id": "c5348c5a-773a-455f-8d75-63b124bc05d5"
            }
          ]
        }
      ]
    },
    {
      "name": "CategoryBuilding",
      "item": [
        {
          "id": "e80affd6-fbda-40e6-86b9-563ef3fac17d",
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
              "id": "01135b24-2fe5-447e-8f87-9abbc940e462"
            }
          ]
        },
        {
          "id": "dc697db1-0367-4cee-b839-33699e8158ec",
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
              "id": "31ee4ebd-0081-427e-9d86-d962072195a3"
            }
          ]
        }
      ]
    },
    {
      "name": "ImagesBuilding",
      "item": [
        {
          "id": "2e756931-e029-4799-bc79-997542af3c29",
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
              "id": "f57b9e14-39b5-4034-8ce1-ed602762b2c3"
            }
          ]
        }
      ]
    },
    {
      "name": "ImageBuilding",
      "item": [
        {
          "id": "8046cd56-3ab8-4c39-b6ab-0e5fd41510da",
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
              "id": "3de73198-0871-4e04-b2f0-9e767b9934b8"
            }
          ]
        },
        {
          "id": "5094a14a-101e-48ba-8979-65d36a416a37",
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
              "id": "cdac45e2-4952-4a6b-938c-5d3c3cfb53e9"
            }
          ]
        }
      ]
    },
    {
      "name": "LogsBuilding",
      "item": [
        {
          "id": "a059ab39-cd72-451a-a08c-4a598b161fe5",
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
              "id": "ce2efb07-ed4c-47f4-88bc-50af4587e6f1"
            }
          ]
        }
      ]
    },
    {
      "name": "LogBuilding",
      "item": [
        {
          "id": "1fc40557-a39d-4814-be1c-832d8ebc4dfb",
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
              "id": "05d07fd2-b85b-4936-8ce5-e62f0e579bee"
            }
          ]
        },
        {
          "id": "d867ce4f-c459-492f-8598-d0c4fdcd4e2a",
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
              "id": "ec2440a1-43ee-49d4-9138-1ea485516ee9"
            }
          ]
        }
      ]
    },
    {
      "name": "OrganizationsBuilding",
      "item": [
        {
          "id": "f1d26513-72c7-4260-8315-36fce0aa1441",
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
              "id": "8cb35857-bcc0-4341-98e6-89d28350a163"
            }
          ]
        }
      ]
    },
    {
      "name": "OrganizationBuilding",
      "item": [
        {
          "id": "42aedbcf-7215-4822-bb92-5704ed81d038",
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
              "id": "86d83261-81f3-4ca4-86d9-8135c4893dab"
            }
          ]
        },
        {
          "id": "7e962c6d-bc95-4a79-b6ee-2a98123b6ec8",
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
              "id": "40ef10de-28c8-4e4f-84c1-408de421e174"
            }
          ]
        }
      ]
    },
    {
      "name": "TagsBuilding",
      "item": [
        {
          "id": "3289acce-d509-4935-87ca-e28fba044db9",
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
              "id": "29849b48-362b-484c-a050-d85cfd3bca33"
            }
          ]
        }
      ]
    },
    {
      "name": "TagBuilding",
      "item": [
        {
          "id": "882e227a-e963-4c34-be39-064b441b5ed5",
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
              "id": "87652f1a-9077-4bcb-9c7d-301e15ea0492"
            }
          ]
        },
        {
          "id": "41efc4f0-311a-4af6-b135-3cd90a2fabf3",
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
              "id": "52bb0736-9b45-4429-ab7c-bd358ff8675e"
            }
          ]
        }
      ]
    },
    {
      "name": "ToolsBuilding",
      "item": [
        {
          "id": "2dc86cdc-018d-48ae-a1bd-c618f6b02104",
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
              "id": "6346f1e5-0185-42c0-bb31-3858b0f504a6"
            }
          ]
        }
      ]
    },
    {
      "name": "ToolBuilding",
      "item": [
        {
          "id": "6b474b87-d283-44d2-88f9-7d16f6df24a0",
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
              "id": "d47b582a-6beb-4a13-b6fc-306b6df990ea"
            }
          ]
        },
        {
          "id": "0e27ca94-b6b3-48cd-a8e5-0aa153ecbea0",
          "name": "getBuildingBlockTool",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/tools/:tool_id"
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
                  "id": "tool_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "delete a building block tool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5829611f-e3d3-497c-80e1-598adb718dea"
            }
          ]
        }
      ]
    },
    {
      "name": "URLsBuilding",
      "item": [
        {
          "id": "28f3e89a-f24d-4f6e-8652-8a3209653140",
          "name": "getbuildingblockURLs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "buildingblock.api.kinlane.com",
              "path": [
                "buildingblocks/:building_block_id/urls/"
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
            "description": "retrieve building block url"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd9e8e08-3818-4489-822c-90684819513a"
            }
          ]
        }
      ]
    }
  ]
}