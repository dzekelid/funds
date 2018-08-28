---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Receipt (optional) and allocate deposit funds to holding account
  version: 1.0.0
  description: Receipt (optional) and allocate deposit funds to holding account.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accountingsystem/suspense:
    get:
      summary: Get amount of funds held in suspense account of the accounting system
      description: Get amount of funds held in suspense account of the accounting
        system.
      operationId: AccountingSystem_GetSuspenseFunds
      x-api-path-slug: apiaccountingsystemsuspense-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Amount
      - Of
      - Funds
      - Held
      - In
      - Suspense
      - Account
      - Of
      - Accounting
      - System
  /api/deposit/allocate:
    post:
      summary: Receipt (optional) and allocate deposit funds to holding account
      description: Receipt (optional) and allocate deposit funds to holding account.
      operationId: Deposit_ReceiptAndAllocateDepositBymoveDataContract
      x-api-path-slug: apidepositallocate-post
      parameters:
      - in: body
        name: moveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Receipt
      - (optional)
      - Ocate
      - Deposit
      - Funds
      - To
      - Holding
      - Account
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---