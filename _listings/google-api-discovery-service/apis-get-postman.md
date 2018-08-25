{
  "info": {
    "name": "Google API Discovery Service API Get APIs",
    "_postman_id": "ef1c528e-6455-420a-9144-bcdde2161762",
    "description": "Retrieve the list of APIs supported at this endpoint.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "API",
      "item": [
        {
          "id": "866334cd-8d75-415f-9466-b3f5d2866739",
          "name": "discovery.apis.list",
          "request": {
            "url": "http://www.googleapis.com/discovery/v1/apis?name=%7B%7D&preferred=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the list of APIs supported at this endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cd2aec4-7916-4fb2-a014-7a81ded0aa76"
            }
          ]
        }
      ]
    }
  ]
}