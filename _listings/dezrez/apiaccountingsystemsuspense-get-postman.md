{
  "info": {
    "name": "Dezrez Get amount of funds held in suspense account of the accounting system",
    "_postman_id": "5d59dcbd-d5ec-4cf8-9409-aae98ba324b9",
    "description": "Get amount of funds held in suspense account of the accounting system.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "System",
      "item": [
        {
          "id": "d70af136-4f5e-420f-bbce-a1dc6f05e10b",
          "name": "Account_GetSystemAccount",
          "request": {
            "url": "http://api.dezrez.com/api/account/systemaccount",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get system account for the accounting system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f08c818-021a-4b6b-b730-900a0eb40d62"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "4bebc616-7fcb-4b2b-8565-535251981088",
          "name": "AccountingSystem_Get",
          "request": {
            "url": "http://api.dezrez.com/api/accountingsystem",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets accounting system for a legal entity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "746a781c-fb8a-42cf-96a1-c97c225f862c"
            }
          ]
        },
        {
          "id": "d2721901-1316-4690-ae37-88a34f6b6dbe",
          "name": "AccountingSystem_GetSystemBalance",
          "request": {
            "url": "http://api.dezrez.com/api/accountingsystem/systembalance",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets accounting system balance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "324c23a9-7c08-46fa-9055-33d8c5f891db"
            }
          ]
        }
      ]
    },
    {
      "name": "Archives",
      "item": [
        {
          "id": "1d051101-7431-49df-83c4-840691092c24",
          "name": "AccountingSystem_ArchiveSystemByforce",
          "request": {
            "url": "http://api.dezrez.com/api/accountingsystem/systembalance?force=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Archives the accounting system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6380bfcc-0767-4e71-b51a-007d094c3b68"
            }
          ]
        }
      ]
    },
    {
      "name": "Tax",
      "item": [
        {
          "id": "bf5073d4-edf7-45e7-8f7d-7e32ae8966de",
          "name": "AccountingSystem_GetTaxStatus",
          "request": {
            "url": "http://api.dezrez.com/api/accountingsystem/taxstatus",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get tax status of accounting system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fde250b1-1a6f-4a23-8ba1-e9a7eb0b85b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Amount",
      "item": [
        {
          "id": "8b929589-c046-42e8-88e8-b122c2bf690c",
          "name": "AccountingSystem_GetSuspenseFunds",
          "request": {
            "url": "http://api.dezrez.com/api/accountingsystem/suspense",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get amount of funds held in suspense account of the accounting system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53a6ba5b-aef3-41f9-b9c8-943ab546a22f"
            }
          ]
        }
      ]
    }
  ]
}