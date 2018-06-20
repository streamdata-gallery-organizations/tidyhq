{
  "info": {
    "name": "API Evangelist Tools API Pull tool",
    "_postman_id": "b25e1261-6ab3-4b47-8992-67bf5aab99df",
    "description": "Returns a list of all tools filtered by keyword.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "668edff3-b1c4-419c-b881-51a3d12a4aac",
      "name": "getTool",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.apievangelist.com",
          "path": [
            "v1",
            "tool/:id"
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
              "id": "id",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns a tool detail"
      },
      "response": [
        {
          "status": "Successful Analysis Response",
          "code": 200,
          "name": "Response_200",
          "id": "73320413-5f8a-4db6-8470-ba06d12b4ad5"
        }
      ]
    },
    {
      "id": "b1d6a615-db70-4833-a651-3eac5cedcd79",
      "name": "getTool",
      "request": {
        "url": "http://api.apievangelist.com/v1/tools/?appid=%7B%7D&appkey=%7B%7D&query=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns a list of all tools filtered by keyword."
      },
      "response": [
        {
          "status": "Successful Analysis Response",
          "code": 200,
          "name": "Response_200",
          "id": "dcb5445b-c4f1-42a5-b62f-2f1cc9bbd16b"
        }
      ]
    }
  ]
}