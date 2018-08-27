---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Adds a new CRM to the system
  version: 1.0.0
  description: Adds a new crm to the system.
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Cart:
    post:
      summary: Adds a new cart to the system
      description: Adds a new cart to the system.
      operationId: Carts_Post
      x-api-path-slug: 3dcartwebapiv1cart-post
      parameters:
      - in: body
        name: cart
        description: A Json or XML object containing the new cart
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Cart
      - To
      - System
  /3dCartWebAPI/v1/Cart/{orderkey}:
    get:
      summary: Get a specific cart
      description: Get a specific cart.
      operationId: Carts_GetCart
      x-api-path-slug: 3dcartwebapiv1cartorderkey-get
      parameters:
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Cart
    put:
      summary: This method is used to update a single cart record in the database.
        The {orderkey} parameter specifies which cart record to update.
      description: This method is used to update a single cart record in the database.
        the {orderkey} parameter specifies which cart record to update..
      operationId: Carts_Update
      x-api-path-slug: 3dcartwebapiv1cartorderkey-put
      parameters:
      - in: body
        name: cart
        description: A Json or XML object containing the cart
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Cart
      - Record
      - In
      - Database
      - ""
      - Orderkey
      - Parameter
      - Specifies
      - Which
      - Cart
      - Record
      - To
      - Update
    delete:
      summary: Delete a Cart in the system
      description: Delete a cart in the system.
      operationId: Carts_Delete
      x-api-path-slug: 3dcartwebapiv1cartorderkey-delete
      parameters:
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Cart
      - In
      - System
  /3dCartWebAPI/v1/Cart/{orderkey}/Item:
    post:
      summary: Adds a new item to a cart
      description: Adds a new item to a cart.
      operationId: Carts_Post
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitem-post
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new cart item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Item
      - To
      - Cart
  /3dCartWebAPI/v1/Cart/{orderkey}/Item/{cartitemid}:
    put:
      summary: Updates a specific item from a specific Cart
      description: Updates a specific item from a specific cart.
      operationId: Carts_Update
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitemcartitemid-put
      parameters:
      - in: path
        name: cartitemid
        description: The unique index ID of an Item
      - in: body
        name: item
        description: A Json or XML object containing the new cart item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Item
      - From
      - Specific
      - Cart
    delete:
      summary: Deletes a CartItem in the system
      description: Deletes a cartitem in the system.
      operationId: Carts_Delete
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitemcartitemid-delete
      parameters:
      - in: path
        name: cartitemid
        description: The unique index ID of an Item
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - CartItem
      - In
      - System
  /3dCartWebAPI/v1/Categories:
    get:
      summary: Get all Categories
      description: Get all categories.
      operationId: Category_GetAllCategories
      x-api-path-slug: 3dcartwebapiv1categories-get
      parameters:
      - in: query
        name: category
        description: Name of the Category
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Categories
    put:
      summary: This method is used to update multiple category records in the database.
        No {categoryid} parameters should be included.
      description: This method is used to update multiple category records in the
        database. no {categoryid} parameters should be included..
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categories-put
      parameters:
      - in: body
        name: categories
        description: A Json or XML object containing the new categories
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Category
      - Records
      - In
      - Database
      - ""
      - "No"
      - Categoryid
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new category to the system
      description: Adds a new category to the system.
      operationId: Category_Post
      x-api-path-slug: 3dcartwebapiv1categories-post
      parameters:
      - in: body
        name: category
        description: A Json or XML object containing the new category
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Category
      - To
      - System
  /3dCartWebAPI/v1/Categories/{categoryid}:
    put:
      summary: This method is used to update a single category record in the database.
        The {categoryid} parameter specifies which category to update.
      description: This method is used to update a single category record in the database.
        the {categoryid} parameter specifies which category to update..
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryid-put
      parameters:
      - in: body
        name: category
        description: A Json or XML object containing the new category
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryid
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Category
      - Record
      - In
      - Database
      - ""
      - Categoryid
      - Parameter
      - Specifies
      - Which
      - Category
      - To
      - Update
  /3dCartWebAPI/v1/Categories/{categoryid}/Options:
    get:
      summary: Get the options from a specific Category
      description: Get the options from a specific category.
      operationId: Category_GetAllCategoryOptions
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-get
      parameters:
      - in: path
        name: categoryid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Options
      - From
      - Specific
      - Category
    put:
      summary: Updates a collection of options from a specific Category
      description: Updates a collection of options from a specific category.
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-put
      parameters:
      - in: path
        name: categoryid
        description: CategoryID
      - in: body
        name: options
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Options
      - From
      - Specific
      - Category
    post:
      summary: Adds a new OptionSet to the system
      description: Adds a new optionset to the system.
      operationId: Category_Post
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-post
      parameters:
      - in: path
        name: categoryid
        description: Category ID
      - in: body
        name: optionset
        description: A Json or XML object containing the new optionset
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - OptionSet
      - To
      - System
  /3dCartWebAPI/v1/Categories/{categoryid}/Options/{optionsetid}:
    put:
      summary: Updates specific options from a specific Category
      description: Updates specific options from a specific category.
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptionsoptionsetid-put
      parameters:
      - in: path
        name: categoryid
        description: CategoryID
      - in: body
        name: option
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionsetid
        description: OptionSetID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Options
      - From
      - Specific
      - Category
  /3dCartWebAPI/v1/Categories/{categoryid}/Products:
    get:
      summary: Get all products from a specific category
      description: Get all products from a specific category.
      operationId: Products_GetAllProductsFromCategory
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidproducts-get
      parameters:
      - in: path
        name: categoryid
        description: ID of the category
      - in: query
        name: categoryspecial
        description: Category Special Flag
      - in: query
        name: costfrom
        description: Cost of a product
      - in: query
        name: costto
        description: Cost of a product
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: freeshipping
        description: Free Shipping Flag
      - in: query
        name: giftcertificate
        description: Gift Certificate Flag
      - in: query
        name: hide
        description: Hide Flag
      - in: query
        name: homespecial
        description: Home Special Flag
      - in: query
        name: lastupdateend
        description: End Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastupdatestart
        description: Start Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: name
        description: Name of the product
      - in: query
        name: nonsearchable
        description: Non-Searchable Flag
      - in: query
        name: nontax
        description: Non-Taxable Flag
      - in: query
        name: notforsale
        description: Not For Sale Flag
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: onsale
        description: On Sale Flag
      - in: query
        name: pricefrom
        description: Price of a product
      - in: query
        name: priceto
        description: Price of a product
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: query
        name: rewarddisable
        description: Disable Rewards Flag
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: selfship
        description: Ships by itself Flag
      - in: query
        name: sku
        description: SKU Code of the product
      - in: query
        name: stockfrom
        description: Stock of a product
      - in: query
        name: stockto
        description: Stock of a product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Products
      - From
      - Specific
      - Category
  /3dCartWebAPI/v1/Categories/{id}:
    get:
      summary: Get a Category
      description: Get a category.
      operationId: Category_GetCategory
      x-api-path-slug: 3dcartwebapiv1categoriesid-get
      parameters:
      - in: path
        name: id
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Category
    delete:
      summary: Deletes a Category in the system
      description: Deletes a category in the system.
      operationId: Category_Delete
      x-api-path-slug: 3dcartwebapiv1categoriesid-delete
      parameters:
      - in: path
        name: id
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
      - In
      - System
  /3dCartWebAPI/v1/CRM:
    get:
      summary: Get all CRMs
      description: Get all crms.
      operationId: CRM_GetAllCRMs
      x-api-path-slug: 3dcartwebapiv1crm-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: custid
        description: Customer Id associated with the CRM
      - in: query
        name: customeremail
        description: Customer Email
      - in: query
        name: customeripaddress
        description: Customer Ip Address
      - in: query
        name: customername
        description: Customer Name
      - in: query
        name: customerphone
        description: Customer Phone
      - in: query
        name: departmentid
        description: Department of the CRM
      - in: query
        name: lastactionenddate
        description: Date Last Action (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastactionstartdate
        description: Date Opened (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: openedenddate
        description: Date Last Action (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: openedstartdate
        description: Date Opened (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: orderid
        description: Order Id associated with the CRM
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: query
        name: productid
        description: Product Id associated with the CRM
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: statusid
        description: Status of the CRM
      - in: query
        name: subject
        description: Subject of the CRM
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CRMs
    post:
      summary: Adds a new CRM to the system
      description: Adds a new crm to the system.
      operationId: CRM_PostCRM
      x-api-path-slug: 3dcartwebapiv1crm-post
      parameters:
      - in: body
        name: crm
        description: A Json or XML object containing the new CRM
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - CRM
      - To
      - System
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