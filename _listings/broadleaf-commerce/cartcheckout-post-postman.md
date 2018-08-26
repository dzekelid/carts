{
  "info": {
    "name": "Broadleaf Commerce API Post Cart Checkout",
    "_postman_id": "17ba509b-befa-47ef-b426-3af1996b3a6a",
    "description": "Post cart checkout.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auditevents",
      "item": [
        {
          "id": "092fe500-ece6-47f5-a26a-20f8ff239e42",
          "name": "getAuditevents",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/auditevents?after=%7B%7D&principal=%7B%7D&type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get auditevents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06e40ee8-0b29-4a1a-9d1e-29a0ddef79fe"
            }
          ]
        },
        {
          "id": "bcc67f95-d535-440b-abe5-851643f33c0a",
          "name": "getAuditevents.json",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/auditevents.json?after=%7B%7D&principal=%7B%7D&type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get auditevents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "116f0559-001d-4132-99b8-e289ee33357c"
            }
          ]
        }
      ]
    },
    {
      "name": "Autoconfig",
      "item": [
        {
          "id": "20b42c42-f8ee-4b26-914c-1b3f33ab0c31",
          "name": "getAutoconfig",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/autoconfig",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get autoconfig."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fe99458-959b-4a64-9772-f75899421fa0"
            }
          ]
        },
        {
          "id": "a125ae19-5e05-4760-aa3d-b94660920843",
          "name": "getAutoconfig.json",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/autoconfig.json",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get autoconfig."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b80302ca-56d6-46be-9780-ce36b00e53ce"
            }
          ]
        }
      ]
    },
    {
      "name": "Beans",
      "item": [
        {
          "id": "6f0a991b-0f15-4429-99fa-e0923fdd4264",
          "name": "getBeans",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/beans",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get beans."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f9b9235-1484-494c-a2e1-396c4834f43d"
            }
          ]
        },
        {
          "id": "d49c048f-79d3-4f66-8237-0d0f764c2e9b",
          "name": "getBeans.json",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/beans.json",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get beans."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d51e1ad2-9474-4cb5-ae35-578172f49899"
            }
          ]
        }
      ]
    },
    {
      "name": "Cart",
      "item": [
        {
          "id": "2b97170e-3dff-478d-81bc-07108f498de1",
          "name": "getCart",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/cart?customerId=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get cart."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9025df7-d416-4348-9e12-6ad9ca2d3e87"
            }
          ]
        },
        {
          "id": "22a9ec86-8f25-4c76-8c2f-5a11f943ed2d",
          "name": "postCart",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/cart?customerId=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Post cart."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fa4acf6-4c70-4130-acc5-3c85275bdc4f"
            }
          ]
        },
        {
          "id": "f58d3dc9-a543-498e-afc6-eac5e016427f",
          "name": "postCartCheckout",
          "request": {
            "url": "http://demo.broadleafcommerce.org/api/v1/cart/checkout?cartId=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Post cart checkout."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48fcc295-5198-4806-b08e-7ea58b3716e8"
            }
          ]
        }
      ]
    }
  ]
}