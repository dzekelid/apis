{
  "info": {
    "name": "APIs.io Get APIS",
    "_postman_id": "a92ac9ce-9fc1-4817-a1dd-72f87e046010",
    "description": "List all the APIs available",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "APIs",
      "item": [
        {
          "id": "5bfeddb3-16c6-4b0b-af85-65a9009d091b",
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
              "id": "2a083692-c29d-4fb8-9440-c3ca98bedb11"
            }
          ]
        }
      ]
    }
  ]
}