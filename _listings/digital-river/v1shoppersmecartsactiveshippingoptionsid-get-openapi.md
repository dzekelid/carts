---
swagger: "2.0"
x-collection-name: Digital River
x-complete: 0
info:
  title: Digital River Shopper API Get Shoppers Me Carts Active Shipping Options
  description: Get shoppers me carts active shipping options.
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/carts/active:
    get:
      summary: Get Shoppers Me Carts Active
      description: Get shoppers me carts active.
      operationId: getV1ShoppersMeCartsActive
      x-api-path-slug: v1shoppersmecartsactive-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
    post:
      summary: Post Shoppers Me Carts Active
      description: Post shoppers me carts active.
      operationId: postV1ShoppersMeCartsActive
      x-api-path-slug: v1shoppersmecartsactive-post
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
  /v1/shoppers/me/carts/active/apply-shipping-option:
    post:
      summary: Post Shoppers Me Carts Active Apply Shipping Option
      description: Post shoppers me carts active apply shipping option.
      operationId: postV1ShoppersMeCartsActiveApplyShippingOption
      x-api-path-slug: v1shoppersmecartsactiveapplyshippingoption-post
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Apply
      - Shipping
      - Option
  /v1/shoppers/me/carts/active/apply-shopper:
    post:
      summary: Post Shoppers Me Carts Active Apply Shopper
      description: Post shoppers me carts active apply shopper.
      operationId: postV1ShoppersMeCartsActiveApplyShopper
      x-api-path-slug: v1shoppersmecartsactiveapplyshopper-post
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Apply
      - Shopper
  /v1/shoppers/me/carts/active/billing-address:
    get:
      summary: Get Shoppers Me Carts Active Billing Address
      description: Get shoppers me carts active billing address.
      operationId: getV1ShoppersMeCartsActiveBillingAddress
      x-api-path-slug: v1shoppersmecartsactivebillingaddress-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Billing
      - Ress
    put:
      summary: Put Shoppers Me Carts Active Billing Address
      description: Put shoppers me carts active billing address.
      operationId: putV1ShoppersMeCartsActiveBillingAddress
      x-api-path-slug: v1shoppersmecartsactivebillingaddress-put
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Billing
      - Ress
  /v1/shoppers/me/carts/active/line-items:
    delete:
      summary: Delete Shoppers Me Carts Active Line Items
      description: Delete shoppers me carts active line items.
      operationId: deleteV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitems-delete
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
    get:
      summary: Get Shoppers Me Carts Active Line Items
      description: Get shoppers me carts active line items.
      operationId: getV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitems-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
    post:
      summary: Post Shoppers Me Carts Active Line Items
      description: Post shoppers me carts active line items.
      operationId: postV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitems-post
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
  /v1/shoppers/me/carts/active/line-items/{id}:
    delete:
      summary: Delete Shoppers Me Carts Active Line Items
      description: Delete shoppers me carts active line items.
      operationId: deleteV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitemsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
    get:
      summary: Get Shoppers Me Carts Active Line Items
      description: Get shoppers me carts active line items.
      operationId: getV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitemsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
    post:
      summary: Post Shoppers Me Carts Active Line Items
      description: Post shoppers me carts active line items.
      operationId: postV1ShoppersMeCartsActiveLineItems
      x-api-path-slug: v1shoppersmecartsactivelineitemsid-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Line
      - Items
  /v1/shoppers/me/carts/active/point-of-promotions/{id}/offers:
    get:
      summary: Get Shoppers Me Carts Active Point Of Promotions Offers
      description: Get shoppers me carts active point of promotions offers.
      operationId: getV1ShoppersMeCartsActivePointOfPromotionsOffers
      x-api-path-slug: v1shoppersmecartsactivepointofpromotionsidoffers-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Point
      - Promotions
      - Offers
  /v1/shoppers/me/carts/active/shipping-address:
    get:
      summary: Get Shoppers Me Carts Active Shipping Address
      description: Get shoppers me carts active shipping address.
      operationId: getV1ShoppersMeCartsActiveShippingAddress
      x-api-path-slug: v1shoppersmecartsactiveshippingaddress-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Shipping
      - Ress
    put:
      summary: Put Shoppers Me Carts Active Shipping Address
      description: Put shoppers me carts active shipping address.
      operationId: putV1ShoppersMeCartsActiveShippingAddress
      x-api-path-slug: v1shoppersmecartsactiveshippingaddress-put
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Shipping
      - Ress
  /v1/shoppers/me/carts/active/shipping-options:
    get:
      summary: Get Shoppers Me Carts Active Shipping Options
      description: Get shoppers me carts active shipping options.
      operationId: getV1ShoppersMeCartsActiveShippingOptions
      x-api-path-slug: v1shoppersmecartsactiveshippingoptions-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Shipping
      - Options
  /v1/shoppers/me/carts/active/shipping-options/{id}:
    get:
      summary: Get Shoppers Me Carts Active Shipping Options
      description: Get shoppers me carts active shipping options.
      operationId: getV1ShoppersMeCartsActiveShippingOptions
      x-api-path-slug: v1shoppersmecartsactiveshippingoptionsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Shipping
      - Options
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