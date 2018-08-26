{
  "info": {
    "name": "Broadleaf Commerce API Post Cart",
    "_postman_id": "46167764-4db3-439b-9598-65a098261a19",
    "description": "Post cart.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auditevents",
      "item": [
        {
          "id": "8e9bc5c3-e4e9-43f5-8d4b-beaa9dacc3ea",
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
              "id": "8e5bc8e3-0517-478f-a802-1f3d996150cb"
            }
          ]
        },
        {
          "id": "46a414be-bb70-4c92-a82c-5fe873e98395",
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
              "id": "b9f93923-0720-46b0-a232-4dbd76e2024b"
            }
          ]
        }
      ]
    },
    {
      "name": "Autoconfig",
      "item": [
        {
          "id": "c9365f11-2c5f-42b3-8a7f-456a737e0eff",
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
              "id": "4ccf2e2c-48c3-4710-9052-6b644e5ba9a6"
            }
          ]
        },
        {
          "id": "27655f48-259d-417a-9110-d1d6264830af",
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
              "id": "880ac4cb-ed2c-4654-8d30-dbbb9cbaaccf"
            }
          ]
        }
      ]
    },
    {
      "name": "Beans",
      "item": [
        {
          "id": "a6e8c827-e24e-4fe5-8ac5-fa9f78ba9b03",
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
              "id": "c871585e-ebea-4cf5-8688-b8a05bc87a61"
            }
          ]
        },
        {
          "id": "f9c644d2-9ded-4eac-88c5-5f28a75f51ca",
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
              "id": "31d10834-8a65-44ab-ab55-e5d39cc80d50"
            }
          ]
        }
      ]
    },
    {
      "name": "Cart",
      "item": [
        {
          "id": "8a95820d-a220-4d75-a820-d0876fe0d78e",
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
              "id": "2a27d04c-b008-4d22-8605-679d574aeb30"
            }
          ]
        },
        {
          "id": "7de59edd-9f6c-4862-b40f-23b17f3f43ee",
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
              "id": "5dd097bc-bb00-4ff8-ae25-36c2aa0b6145"
            }
          ]
        }
      ]
    }
  ]
}