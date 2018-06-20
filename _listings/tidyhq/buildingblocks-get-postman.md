{
  "info": {
    "name": "API Evangelist Building Block API Get All Building Blocks",
    "_postman_id": "77edbeed-4a95-4f39-85d6-ac7692733cc3",
    "description": "all building blocks",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Building",
      "item": [
        {
          "id": "58e6ab63-0a56-431a-ae42-503dcdf346a0",
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
              "id": "5e6835d1-cb41-4ee9-b941-88b7bd82515b"
            }
          ]
        }
      ]
    }
  ]
}