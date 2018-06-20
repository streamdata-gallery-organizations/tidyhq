{
  "info": {
    "name": "API Evangelist Building Block API Delete Tag for Building Block",
    "_postman_id": "9ad5555f-a509-479f-90c6-f2f41b2294c2",
    "description": "delete buildingblock tag",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Building",
      "item": [
        {
          "id": "f91e873c-5af2-4788-91f8-4be7103824ff",
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
              "id": "71eda93b-124b-4063-af72-ed1d20a4fb6d"
            }
          ]
        },
        {
          "id": "f712f1b8-641d-4784-baf2-19a494c2b8f1",
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
              "id": "2e9f1cd6-00e5-4566-a4d2-cd7a4eda356d"
            }
          ]
        },
        {
          "id": "0a2fc6de-4be7-49d6-b39b-b2c1a9042172",
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
              "id": "9128b224-2998-47bc-8703-b223e133220d"
            }
          ]
        },
        {
          "id": "d6846315-a136-4d08-8fcd-2866973803ef",
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
              "id": "2cb2748f-ada9-43fc-ad37-e94c97c83ae6"
            }
          ]
        },
        {
          "id": "e82a6d16-bcb2-45dc-80f8-3ec0f32ab1fa",
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
              "id": "38afa327-abbc-4b1b-ade5-4a5dae7494c3"
            }
          ]
        },
        {
          "id": "8388545f-2ce8-4727-bf62-d12a1c5f6581",
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
              "id": "51b5d2f1-d528-4ef9-bcbb-da31eaf1f3fe"
            }
          ]
        },
        {
          "id": "50e79917-02af-447f-9da1-bebd2ce25f05",
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
              "id": "77f4d5ac-57da-4269-b5d2-73b111863207"
            }
          ]
        }
      ]
    },
    {
      "name": "CategoriesBuilding",
      "item": [
        {
          "id": "e58fafd7-0ec7-447e-a15a-3563cc33246a",
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
              "id": "aa126790-61a8-4731-8373-abfba8a697ca"
            }
          ]
        }
      ]
    },
    {
      "name": "CategoryBuilding",
      "item": [
        {
          "id": "1f3062a1-0235-4709-b2d8-6538caac34ae",
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
              "id": "e07f426e-7b20-493f-8767-c4fbe522a704"
            }
          ]
        },
        {
          "id": "8efc7357-8a66-41c4-88ef-8df39ee07878",
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
              "id": "5fe0c061-f98a-48c8-8853-94da58200806"
            }
          ]
        }
      ]
    },
    {
      "name": "ImagesBuilding",
      "item": [
        {
          "id": "db011b4e-c6db-4ecd-82bf-6f2a9544d8fc",
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
              "id": "0f07b2a8-06d8-42e7-922b-addc82303c20"
            }
          ]
        }
      ]
    },
    {
      "name": "ImageBuilding",
      "item": [
        {
          "id": "48b79f6b-d776-41b5-9dff-0deedbc02198",
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
              "id": "156cf9e8-3577-4497-8f14-7fd2a97cf562"
            }
          ]
        },
        {
          "id": "0d026d8e-0b05-442c-9266-fa82768b6553",
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
              "id": "a092d528-a872-4e21-9dc9-759d3f6cc647"
            }
          ]
        }
      ]
    },
    {
      "name": "LogsBuilding",
      "item": [
        {
          "id": "3724412f-245b-484d-a8c1-a67499c58183",
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
              "id": "6cd43366-b838-4b81-9993-a0fe82936946"
            }
          ]
        }
      ]
    },
    {
      "name": "LogBuilding",
      "item": [
        {
          "id": "c8db8e9f-0cb9-490b-981d-6cadca84a248",
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
              "id": "d42f21ec-5584-4c54-9343-fed78ac72dc3"
            }
          ]
        },
        {
          "id": "d657a2be-a3bc-4ad5-9103-f50faa645a04",
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
              "id": "33811eb3-e1f2-40cc-b5a9-c9dcaf358ffd"
            }
          ]
        }
      ]
    },
    {
      "name": "OrganizationsBuilding",
      "item": [
        {
          "id": "11ed5cfb-28e3-4c5f-9715-df3f03123a8d",
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
              "id": "7ebcc9cd-865f-4dc7-bc5f-444da042f9ce"
            }
          ]
        }
      ]
    },
    {
      "name": "OrganizationBuilding",
      "item": [
        {
          "id": "0ed47b9d-25ba-405c-b053-1e3297cfda96",
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
              "id": "1ae6009a-f208-4b73-9f5f-f787d82ea7bb"
            }
          ]
        },
        {
          "id": "d441901f-af12-4d84-81de-060947d093a5",
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
              "id": "63d82fe7-2641-4a13-ad01-429388f11d40"
            }
          ]
        }
      ]
    },
    {
      "name": "TagsBuilding",
      "item": [
        {
          "id": "6302d043-9c0e-4b4c-9227-3f88f880fc39",
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
              "id": "68fac92f-4543-4c4a-98bc-cbfbe774c469"
            }
          ]
        }
      ]
    },
    {
      "name": "TagBuilding",
      "item": [
        {
          "id": "e598d617-446b-489a-9ac7-5f1cdd48ca15",
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
              "id": "4251d90f-1906-4b6e-a45d-80b8f125cebd"
            }
          ]
        },
        {
          "id": "522e8c09-4214-4fe2-9a42-6203efeb5e20",
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
              "id": "01458408-c415-452a-b191-aa486ca3e7e6"
            }
          ]
        }
      ]
    }
  ]
}