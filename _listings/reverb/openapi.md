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
  /cart:
    get:
      summary: Get Cart
      description: Get all cart items
      operationId: getCart
      x-api-path-slug: cart-get
      responses:
        200:
          description: OK
      tags:
      - Cart
  /cart/move_to_watch_list/{cart_item_id}:
    post:
      summary: Post Cart Move To Watch List Cart Item
      description: Remove a cart item and add it to watch list
      operationId: postCartMoveToWatchListCartItem
      x-api-path-slug: cartmove-to-watch-listcart-item-id-post
      parameters:
      - in: path
        name: cart_item_id
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Move
      - To
      - Watch
      - List
      - Cart
      - Item
      - Id
  /cart/{id}:
    delete:
      summary: Delete Cart
      description: Remove a product from the cart
      operationId: deleteCart
      x-api-path-slug: cartid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Id
    post:
      summary: Post Cart
      description: Add product to the cart
      operationId: postCart
      x-api-path-slug: cartid-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Id
    put:
      summary: Put Cart
      description: Update cart item details
      operationId: putCart
      x-api-path-slug: cartid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Id
---