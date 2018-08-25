{
  "info": {
    "name": "APIs.io Search APIs",
    "_postman_id": "04dbdc4d-7a4a-447a-922a-ec878a0f587a",
    "description": "Search for apis",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "APIs",
      "item": [
        {
          "id": "31e86d03-ee60-4ce9-b840-669c53699d54",
          "name": "getAPIs",
          "request": {
            "url": "http://apis.io/api/apis?fields=fields&q=q",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all the APIs available"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8a8503e-ee5b-46a8-9466-57967a3f0b95"
            }
          ]
        },
        {
          "id": "fe4a5ec1-28f2-415b-8071-0da189bb7fee",
          "name": "searchAPIs",
          "request": {
            "url": "http://apis.io/api/search",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for apis"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3f36743-bec4-4085-b285-d4681c1025a4"
            }
          ]
        }
      ]
    }
  ]
}