{
  "info": {
    "name": "Instructure Canvas Utility APIs Show an outcome",
    "_postman_id": "ffec4605-1d13-4355-b677-af1ee25b832f",
    "description": "Show an outcome.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Api",
      "item": [
        {
          "id": "98360b04-85a2-4d62-990e-5151b8bccd6f",
          "name": "retrieve-assignments-enabled-for-grade-export-to-sis",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "api/sis/accounts/:account_id/assignments"
              ],
              "query": [
                {
                  "key": "course_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ends_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starts_before",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve assignments enabled for grade export to sis."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e505a99e-9365-47ff-9dd9-ef0bc64a7057"
            }
          ]
        },
        {
          "id": "7943d35c-0929-40ae-a5f2-98fef7ad6a42",
          "name": "retrieve-assignments-enabled-for-grade-export-to-sis1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "api/sis/courses/:course_id/assignments"
              ],
              "query": [
                {
                  "key": "account_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ends_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starts_before",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve assignments enabled for grade export to sis."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcf16eb4-edf3-43d7-afd1-46be62f4f235"
            }
          ]
        }
      ]
    },
    {
      "name": "Collaborations",
      "item": [
        {
          "id": "12ff4c10-3d1d-47ee-81e2-37d558da1cf4",
          "name": "list-members-of-a-collaboration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "collaborations/:id/members"
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
            "description": "List members of a collaboration.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83f03cc9-9ab5-476a-9ecc-5b92c61bea7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Comm",
      "item": [
        {
          "id": "897f6ad4-bd85-47c6-950b-a3d97525cd93",
          "name": "list-of-commmessages-for-a-user",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/comm_messages?end_time=%7B%7D&start_time=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of commmessages for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7d0773b-5717-406d-8a50-6fcd83eb2160"
            }
          ]
        }
      ]
    },
    {
      "name": "Outcomes",
      "item": [
        {
          "id": "d6eecd4f-9391-4a93-a3d9-fcefaeda2456",
          "name": "show-an-outcome",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "outcomes/:id"
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
            "description": "Show an outcome."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e802e105-5ba4-41b6-b779-bd0b277d3fd6"
            }
          ]
        }
      ]
    }
  ]
}