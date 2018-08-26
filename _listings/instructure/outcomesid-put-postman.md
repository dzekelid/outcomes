{
  "info": {
    "name": "Instructure Canvas Utility APIs Update an outcome",
    "_postman_id": "8e28eb6d-8162-4767-9e2f-79ca0374247a",
    "description": "Update an outcome.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Api",
      "item": [
        {
          "id": "ce13bd05-c3b8-4649-8896-4e244c800145",
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
              "id": "3029275a-df1a-4989-9a63-8c84f976aac5"
            }
          ]
        },
        {
          "id": "809e8223-bdb4-4b43-b47e-c2048fb6085b",
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
              "id": "6c326f5b-563d-4564-976c-53738eaf5987"
            }
          ]
        }
      ]
    },
    {
      "name": "Collaborations",
      "item": [
        {
          "id": "6585c3bd-be91-4944-8b46-564fae9372b1",
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
              "id": "f27d70d4-e8c3-478f-bac9-2294313fa0b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Comm",
      "item": [
        {
          "id": "a9124e22-fa64-43ae-b99b-18d942b50423",
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
              "id": "37323ba1-a2e9-4943-a803-29c76f851f34"
            }
          ]
        }
      ]
    },
    {
      "name": "Outcomes",
      "item": [
        {
          "id": "06b06492-0755-41da-938e-f187fa0e4815",
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
              "id": "1805f636-975c-4364-bcb0-98a9ac908ad6"
            }
          ]
        },
        {
          "id": "e32da3f9-ae7b-4460-a9f7-24e8427383aa",
          "name": "update-an-outcome",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "outcomes/:id"
              ],
              "query": [
                {
                  "key": "calculation_int",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calculation_method",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "display_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "mastery_points",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ratings[][description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ratings[][points]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "vendor_guid",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an outcome."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0298d5b4-d325-4777-9f2f-39ff972b7a0c"
            }
          ]
        }
      ]
    }
  ]
}