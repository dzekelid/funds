swagger: "2.0"
x-collection-name: Envestnet
x-complete: 1
info:
  title: Crunch Base
  description: the-crunchbase-api-is-a-relatively-straightforward-rest-service-that-allows-developers-to-access-data-in-the-business-graph-
  termsOfService: https://data.crunchbase.com/v3/page/accessing-the-dataset
  contact:
    name: Crunchbase
    url: https://groups.google.com/forum/#!forum/crunchbase-api
    email: data@crunchbase.com
  version: v3
host: api.crunchbase.com
basePath: /v/3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /funds/:uuid/{relationship_name}:
    get:
      summary: Get Fund Relationships
      description: Get Fund Relationships
      operationId: fundRelationships
      x-api-path-slug: fundsuuidrelationship-name-get
      parameters:
      - in: query
        name: page
        description: The number of the page to retrieve
      - in: path
        name: relationship_name
        description: The name of the connection between the Fund and related Items
      - in: query
        name: sort_order
        description: The sort order
      - in: path
        name: uuid
        description: The 32-character identifier of the Fund
      responses:
        200:
          description: OK
      tags:
      - Funds
      - :uuid
      - Relationship
      - Name
  /funds/{uuid}:
    get:
      summary: Get Funds
      description: Get Funds
      operationId: funds
      x-api-path-slug: fundsuuid-get
      parameters:
      - in: path
        name: uuid
        description: The UUID of the Fund Raise
      responses:
        200:
          description: OK
      tags:
      - Funds
      - Uuid