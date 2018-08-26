---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shops/{id}/storefronts:
    get:
      summary: Get Shops Storefronts
      description: Get storefront details on a shop.
      operationId: getShopsStorefronts
      x-api-path-slug: shopsidstorefronts-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Id
      - Storefronts
---