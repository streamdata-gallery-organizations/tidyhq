{
  "info": {
    "name": "API Evangelist Building Block API Add Building Block",
    "_postman_id": "5355cb95-0ed5-43ca-8212-6596f481ae27",
    "description": "add a building block post",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Building",
      "item": [
        {
          "id": "548641ee-3798-4294-be57-379542f27ba2",
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
              "id": "ffc9fc9c-becf-4c58-9eb7-6675eac232ef"
            }
          ]
        },
        {
          "id": "2423184b-fc38-4ad8-9ac1-ac145ac1b0e7",
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
              "id": "d9c4cd93-2cff-4ec5-a89d-ee3d153feb25"
            }
          ]
        }
      ]
    }
  ]
}