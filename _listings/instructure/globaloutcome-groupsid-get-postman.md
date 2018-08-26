{
  "info": {
    "name": "Instructure Canvas Global API Show an outcome group",
    "_postman_id": "0a9ab37a-a1b7-42b3-bb62-9677acb96499",
    "description": "Show an outcome group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Global",
      "item": [
        {
          "id": "43818660-b8ce-4fbe-9187-6b65fccd9227",
          "name": "show-an-outcome-group",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e946bb7-c00e-451f-9860-421b0c8cfb0d"
            }
          ]
        },
        {
          "id": "82af0fcc-7ccd-40d8-91b2-8bfb112f128f",
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
              "id": "9a913eaf-1a83-46fd-b96c-f7bb04ab5cd4"
            }
          ]
        }
      ]
    }
  ]
}