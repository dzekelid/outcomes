{
  "info": {
    "name": "Instructure Canvas Global API Delete an outcome group",
    "_postman_id": "a06f4fe4-c704-4231-9b3b-fc5e913adcbf",
    "description": "Delete an outcome group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Global",
      "item": [
        {
          "id": "739866f9-9bf0-4f3c-b03c-9a22353dfe49",
          "name": "delete-an-outcome-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "global/outcome_groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2b61aba-de7b-4496-9b4f-4dc501425c90"
            }
          ]
        }
      ]
    }
  ]
}