{
  "info": {
    "name": "APIs.io Add APIs",
    "_postman_id": "86e623ab-43aa-453a-8e48-e489edf51dea",
    "description": "Adds an API to APIs.io",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "APIs",
      "item": [
        {
          "id": "0d22e70b-e839-4e83-830b-857bd9d0ef61",
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
              "id": "ddfcf496-b2e2-4680-96b4-853b50724cf3"
            }
          ]
        },
        {
          "id": "193c8dd7-d88d-4157-a912-94ff9ace8d88",
          "name": "addAPI",
          "request": {
            "url": "http://apis.io/api/apis?url=url",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an API to APIs.io"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dabc7fe3-a03f-4378-aad3-f91ac8d2ebe9"
            }
          ]
        },
        {
          "id": "ad5d8c96-7eca-4aa3-b116-9d01942679ca",
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
              "id": "e64e09a5-7b19-477c-8f4c-ac11f28d4b69"
            }
          ]
        }
      ]
    }
  ]
}