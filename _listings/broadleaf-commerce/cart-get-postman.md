{
  "info": {
    "name": "Broadleaf Commerce API Get Cart",
    "_postman_id": "ce89fbbe-947a-4091-ab22-b4ca636ee25e",
    "description": "Get cart.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Auditevents",
      "item": [
        {
          "id": "2bd4e1db-60da-4bd6-934d-b58672340bb3",
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
              "id": "e72dd27a-00cd-4130-934b-518c8d566fad"
            }
          ]
        },
        {
          "id": "ae3bba58-e6b3-4c71-a93e-029e1cd2687b",
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
              "id": "13778ece-5570-4ea1-a8d0-0a0148d9d66c"
            }
          ]
        }
      ]
    },
    {
      "name": "Autoconfig",
      "item": [
        {
          "id": "8ca301a4-4ad6-40ae-913b-09f635f36cd7",
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
              "id": "66b46cc8-6472-4cfb-987d-aff19d505861"
            }
          ]
        },
        {
          "id": "79b5360a-55c8-4a3c-b2b4-d8f8ad849db4",
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
              "id": "190081d8-9814-4f94-a57d-8f7dd8da3329"
            }
          ]
        }
      ]
    },
    {
      "name": "Beans",
      "item": [
        {
          "id": "7300c4ba-c168-487c-b5bf-b1f4a23d610a",
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
              "id": "9aab52c9-7941-4315-9871-aac8c109777c"
            }
          ]
        },
        {
          "id": "035e3375-e0c1-48bb-95aa-471d04606f1c",
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
              "id": "246681f4-04ba-4616-8278-0373bb32a815"
            }
          ]
        }
      ]
    },
    {
      "name": "Cart",
      "item": [
        {
          "id": "b541a594-af61-4800-bac9-9a1154e61297",
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
              "id": "af2f44d3-bd09-4e27-8d13-e2b8e823989a"
            }
          ]
        }
      ]
    }
  ]
}