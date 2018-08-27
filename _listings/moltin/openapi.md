swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/v2/carts/{CART_REFERENCE} ':
    delete:
      summary: Delete Cart
      description: |-
        Update an existing item in a cart. The updated cart contents are returned if the call is successful.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart **OR** productID.

        When updating custom itesm you must use the identifier in the cart - you can update more properties of a custom cart item.
      operationId: V2CartsByCARTREFERENCEDelete
      x-api-path-slug: v2cartscart-reference-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: CART_REFERENCE
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Cart
  /v2/carts/123456/items:
    get:
      summary: Get the items in a cart
      description: Get the items in a cart.
      operationId: V2Carts123456ItemsGet
      x-api-path-slug: v2carts123456items-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Items
      - Cart
    post:
      summary: Add a promotion to a cart
      description: |-
        Update an existing item in a cart. The updated cart contents are returned if the call is successful.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart **OR** productID.

        When updating custom itesm you must use the identifier in the cart - you can update more properties of a custom cart item.
      operationId: V2Carts123456ItemsPost2
      x-api-path-slug: v2carts123456items-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
      - To
      - Cart
  /v2/carts/123456:
    get:
      summary: Get a Cart
      description: Get a cart.
      operationId: V2Carts123456Get
      x-api-path-slug: v2carts123456-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Cart
  /v2/carts/123456/items/{itemID}:
    put:
      summary: Update an item in a cart
      description: |-
        Update an existing item in a cart. The updated cart contents are returned if the call is successful.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart **OR** productID.

        When updating custom itesm you must use the identifier in the cart - you can update more properties of a custom cart item.
      operationId: V2Carts123456ItemsByItemIDPut
      x-api-path-slug: v2carts123456itemsitemid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: itemID
      responses:
        200:
          description: Successful response
      tags:
      - Item
      - Cart
  /v2/carts/123456/items/{cartItemID}:
    delete:
      summary: Delete an item from a cart
      description: |-
        Delete an item from a cart. The remaining cart contents are returned on a successful delete.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart rather than the product_id
      operationId: V2Carts123456ItemsByCartItemIDDelete
      x-api-path-slug: v2carts123456itemscartitemid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cartItemID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Item
      - From
      - Cart
  /carts/{cartRef}:
    delete:
      summary: Delete a Cart
      description: Removes all items in a cart.
      operationId: CartsByCartRefDelete
      x-api-path-slug: cartscartref-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cartRef
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Cart