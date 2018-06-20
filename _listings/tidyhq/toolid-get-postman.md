{
  "info": {
    "name": "API Evangelist Tools API Retrieve a tool using its ID",
    "_postman_id": "a31099fa-4748-4d84-84b0-a02576365c1b",
    "description": "Returns a tool detail",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "5860288c-7d65-494e-9d71-e9f5ed2b8596",
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
          "id": "e74ca5b0-4f2c-4755-9e79-5f7527622941"
        }
      ]
    }
  ]
}