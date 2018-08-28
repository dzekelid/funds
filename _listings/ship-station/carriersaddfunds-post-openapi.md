---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station Add Funds
  description: |-
    Adds funds to a carrier account using the payment information on file. The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
     ``carrierCode`` | string, required |  The carrier to add funds to.
     ``amount`` | number, required | The dollar amount to add to the account.  The minimum value that can be added is $10.00.  The maximum value is $10,000.00.
  version: 1.0.0
host: ssapi.shipstation.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /carriers/addfunds:
    post:
      summary: Add Funds
      description: |-
        Adds funds to a carrier account using the payment information on file. The body of this request should specify the following attributes:

        Name               |Data Type          |Description
        -------------------|-------------------|-------------------
         ``carrierCode`` | string, required |  The carrier to add funds to.
         ``amount`` | number, required | The dollar amount to add to the account.  The minimum value that can be added is $10.00.  The maximum value is $10,000.00.
      operationId: carriers.addfunds.post
      x-api-path-slug: carriersaddfunds-post
      responses:
        200:
          description: OK
      tags:
      - Funds
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