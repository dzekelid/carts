---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Get all products from a specific distributor
  version: 1.0.0
  description: Get all products from a specific distributor.
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
  /3dCartWebAPI/v1/CRM/department:
    get:
      summary: Get all CRM Departments
      description: Get all crm departments.
      operationId: CRM_GetAllCRMDepartments
      x-api-path-slug: 3dcartwebapiv1crmdepartment-get
      parameters:
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
      - CRM
      - Departments
  /3dCartWebAPI/v1/CRM/department/{id}:
    put:
      summary: This method is used to update a single CRM Department record in the
        database. The {id} parameter specifies which CRM Department record to update.
      description: This method is used to update a single crm department record in
        the database. the {id} parameter specifies which crm department record to
        update..
      operationId: CRM_UpdateDepartment
      x-api-path-slug: 3dcartwebapiv1crmdepartmentid-put
      parameters:
      - in: body
        name: department
        description: A Json or XML object containing the new Department
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Department ID
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
      - CRM
      - Department
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - Department
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/CRM/savedreply:
    get:
      summary: Get all CRMs
      description: Get all crms.
      operationId: CRM_GetAllCRMSavedReplies
      x-api-path-slug: 3dcartwebapiv1crmsavedreply-get
      parameters:
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
      - in: query
        name: title
        description: Title
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CRMs
    post:
      summary: Adds a new CRM SaveReply to the system
      description: Adds a new crm savereply to the system.
      operationId: CRM_PostSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreply-post
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: savereply
        description: A Json or XML object containing the new CRM SavedReply
        schema:
          $ref: '#/definitions/holder'
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
      - SaveReply
      - To
      - System
  /3dCartWebAPI/v1/CRM/savedreply/{id}:
    get:
      summary: Get a specific CRM Saved Reply
      description: Get a specific crm saved reply.
      operationId: CRM_GetCRMSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreplyid-get
      parameters:
      - in: path
        name: id
        description: CRM Saved Reply ID
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
      - CRM
      - Saved
      - Reply
    put:
      summary: This method is used to update a single CRM SavedReply record in the
        database. The {id} parameter specifies which CRM SavedReply record to update.
      description: This method is used to update a single crm savedreply record in
        the database. the {id} parameter specifies which crm savedreply record to
        update..
      operationId: CRM_UpdateSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreplyid-put
      parameters:
      - in: path
        name: id
        description: SavedReply ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: savedreply
        description: A Json or XML object containing the new SavedReply
        schema:
          $ref: '#/definitions/holder'
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
      - CRM
      - SavedReply
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - SavedReply
      - Record
      - To
      - Update
    delete:
      summary: Delete a CRM SavedReply in the system
      description: Delete a crm savedreply in the system.
      operationId: CRM_DeleteCRMSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreplyid-delete
      parameters:
      - in: path
        name: id
        description: SavedReplyID
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
      - CRM
      - SavedReply
      - In
      - System
  /3dCartWebAPI/v1/CRM/status:
    get:
      summary: Get all CRM Status
      description: Get all crm status.
      operationId: CRM_GetAllCRMStatus
      x-api-path-slug: 3dcartwebapiv1crmstatus-get
      parameters:
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
      - CRM
      - Status
  /3dCartWebAPI/v1/CRM/status/{id}:
    put:
      summary: This method is used to update a single CRM Status record in the database.
        The {id} parameter specifies which CRM Status record to update.
      description: This method is used to update a single crm status record in the
        database. the {id} parameter specifies which crm status record to update..
      operationId: CRM_UpdateStatus
      x-api-path-slug: 3dcartwebapiv1crmstatusid-put
      parameters:
      - in: path
        name: id
        description: Status ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: status
        description: A Json or XML object containing the new Status
        schema:
          $ref: '#/definitions/holder'
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
      - CRM
      - Status
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - Status
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/CRM/{crmid}/message:
    get:
      summary: Get all the messages from a specific CRM
      description: Get all the messages from a specific crm.
      operationId: CRM_GetAllCRMMessages
      x-api-path-slug: 3dcartwebapiv1crmcrmidmessage-get
      parameters:
      - in: path
        name: crmid
        description: CRM ID
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
      - Messages
      - From
      - Specific
      - CRM
  /3dCartWebAPI/v1/CRM/{crmid}/message/{msgid}:
    get:
      summary: Get a specific Message
      description: Get a specific message.
      operationId: CRM_GetCRMMessage
      x-api-path-slug: 3dcartwebapiv1crmcrmidmessagemsgid-get
      parameters:
      - in: path
        name: crmid
        description: CRM ID
      - in: path
        name: msgid
        description: Message ID
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
      - Message
    delete:
      summary: Delete a CRM Message in the system
      description: Delete a crm message in the system.
      operationId: CRM_DeleteCRM
      x-api-path-slug: 3dcartwebapiv1crmcrmidmessagemsgid-delete
      parameters:
      - in: path
        name: crmid
        description: CrmID
      - in: path
        name: msgid
        description: MessageID
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
      - CRM
      - Message
      - In
      - System
  /3dCartWebAPI/v1/CRM/{id}:
    get:
      summary: Get a specific CRM
      description: Get a specific crm.
      operationId: CRM_GetCRM
      x-api-path-slug: 3dcartwebapiv1crmid-get
      parameters:
      - in: path
        name: id
        description: CRM ID
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
      - CRM
    put:
      summary: This method is used to update a single CRM record in the database.
        The {id} parameter specifies which CRM record to update.
      description: This method is used to update a single crm record in the database.
        the {id} parameter specifies which crm record to update..
      operationId: CRM_UpdateCRM
      x-api-path-slug: 3dcartwebapiv1crmid-put
      parameters:
      - in: body
        name: crm
        description: A Json or XML object containing the new product
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Crm ID
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
      - CRM
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - Record
      - To
      - Update
    delete:
      summary: Delete a CRM in the system
      description: Delete a crm in the system.
      operationId: CRM_DeleteCRM
      x-api-path-slug: 3dcartwebapiv1crmid-delete
      parameters:
      - in: path
        name: id
        description: CrmID
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
      - CRM
      - In
      - System
  /3dCartWebAPI/v1/CRM/{id}/message:
    post:
      summary: Adds a new CRM Message to the system
      description: Adds a new crm message to the system.
      operationId: CRM_PostMessage
      x-api-path-slug: 3dcartwebapiv1crmidmessage-post
      parameters:
      - in: path
        name: id
        description: Id of the CRM where the message will be added
      - in: body
        name: message
        description: A Json or XML object containing the new CRM message
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
      - Message
      - To
      - System
  /3dCartWebAPI/v1/CustomerGroups:
    get:
      summary: Get all CustomerGroups
      description: Get all customergroups.
      operationId: CustomerGroups_GetAllCustomerGroups
      x-api-path-slug: 3dcartwebapiv1customergroups-get
      parameters:
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
      - CustomerGroups
    put:
      summary: This method updates a collection of customer groups in the database.
        No URL parameters should be included.
      description: This method updates a collection of customer groups in the database.
        no url parameters should be included..
      operationId: CustomerGroups_Update
      x-api-path-slug: 3dcartwebapiv1customergroups-put
      parameters:
      - in: body
        name: customergroups
        description: A Json or XML object containing the customer group
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
      - Updates
      - Collection
      - Of
      - Customer
      - Groups
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new customer group to the system
      description: Adds a new customer group to the system.
      operationId: CustomerGroups_Post
      x-api-path-slug: 3dcartwebapiv1customergroups-post
      parameters:
      - in: body
        name: customergroup
        description: A Json or XML object containing the new customer group
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
      - Customer
      - Group
      - To
      - System
  /3dCartWebAPI/v1/CustomerGroups/{customergroupid}:
    put:
      summary: This method is used to update a single customer group in the database.
        The {id} parameter specifies which customer group to update.
      description: This method is used to update a single customer group in the database.
        the {id} parameter specifies which customer group to update..
      operationId: CustomerGroups_Update
      x-api-path-slug: 3dcartwebapiv1customergroupscustomergroupid-put
      parameters:
      - in: body
        name: customergroup
        description: A Json or XML object containing the customer group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customergroupid
        description: Customer Group ID
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
      - Customer
      - Group
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - Customer
      - Group
      - To
      - Update
  /3dCartWebAPI/v1/CustomerGroups/{id}:
    get:
      summary: Get a CustomerGroup
      description: Get a customergroup.
      operationId: CustomerGroups_GetCustomerGroup
      x-api-path-slug: 3dcartwebapiv1customergroupsid-get
      parameters:
      - in: path
        name: id
        description: Customer Group ID
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
      - CustomerGroup
    delete:
      summary: Deletes a customer group in the system
      description: Deletes a customer group in the system.
      operationId: CustomerGroups_Delete
      x-api-path-slug: 3dcartwebapiv1customergroupsid-delete
      parameters:
      - in: path
        name: id
        description: Customer Group ID
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
      - Customer
      - Group
      - In
      - System
  /3dCartWebAPI/v1/CustomerGroups/{id}/Customers:
    get:
      summary: Get Customers from a Customer Group
      description: Get customers from a customer group.
      operationId: Customers_GetCustomerFromCustomerGroup
      x-api-path-slug: 3dcartwebapiv1customergroupsidcustomers-get
      parameters:
      - in: query
        name: city
        description: City of the Customer
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: country
        description: Country name of the Customer
      - in: query
        name: email
        description: Email of the Customer
      - in: query
        name: firstname
        description: Firstname of the Customer
      - in: path
        name: id
        description: Customer Group ID
      - in: query
        name: lastname
        description: Lastname of the Customer
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
        name: offset
        description: Starting point for the return data
      - in: query
        name: phone
        description: Phone of the Customer
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: state
        description: State of the Customer
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Customers
      - From
      - Customer
      - Group
  /3dCartWebAPI/v1/Customers:
    get:
      summary: Get all Customers
      description: Get all customers.
      operationId: Customers_GetAllCustomers
      x-api-path-slug: 3dcartwebapiv1customers-get
      parameters:
      - in: query
        name: city
        description: City of the Customer
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: country
        description: Country name of the Customer
      - in: query
        name: email
        description: Email of the Customer
      - in: query
        name: firstname
        description: Firstname of the Customer
      - in: query
        name: lastname
        description: Lastname of the Customer
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
        name: offset
        description: Starting point for the return data
      - in: query
        name: phone
        description: Phone of the Customer
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: state
        description: State of the Customer
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Customers
    put:
      summary: This method is used to update multiple customers in the system. No
        URL parameters should be included.
      description: This method is used to update multiple customers in the system.
        no url parameters should be included..
      operationId: Customers_Update
      x-api-path-slug: 3dcartwebapiv1customers-put
      parameters:
      - in: body
        name: customers
        description: A Json or XML object containing the new customer
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
      - Customers
      - In
      - System
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new customer to the system
      description: Adds a new customer to the system.
      operationId: Customers_Post
      x-api-path-slug: 3dcartwebapiv1customers-post
      parameters:
      - in: body
        name: customer
        description: A Json or XML object containing the new customer
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
      - Customer
      - To
      - System
  /3dCartWebAPI/v1/Customers/{customerid}:
    put:
      summary: This method is used to update a single customer record in the database.
        The {id} parameter specifies which customer record to update.
      description: This method is used to update a single customer record in the database.
        the {id} parameter specifies which customer record to update..
      operationId: Customers_Update
      x-api-path-slug: 3dcartwebapiv1customerscustomerid-put
      parameters:
      - in: body
        name: customer
        description: A Json or XML object containing the new customer
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerid
        description: Customer ID
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
      - Customer
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - Customer
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Customers/{id}:
    get:
      summary: Get a Customer
      description: Get a customer.
      operationId: Customers_GetAllCustomers
      x-api-path-slug: 3dcartwebapiv1customersid-get
      parameters:
      - in: path
        name: id
        description: Customer ID
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
      - Customer
    delete:
      summary: Deletes a Customer in the system
      description: Deletes a customer in the system.
      operationId: Customers_Delete
      x-api-path-slug: 3dcartwebapiv1customersid-delete
      parameters:
      - in: path
        name: id
        description: Customer ID
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
      - Customer
      - In
      - System
  /3dCartWebAPI/v1/Distributors:
    get:
      summary: Get all Distributors
      description: Get all distributors.
      operationId: Distributors_GetAllDistributors
      x-api-path-slug: 3dcartwebapiv1distributors-get
      parameters:
      - in: query
        name: city
        description: City of the Distributor
      - in: query
        name: company
        description: Company Name of the Distributor
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: country
        description: Country name of the Distributor
      - in: query
        name: email
        description: Email of the Distributor
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: phone
        description: Phone of the Distributor
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: state
        description: State of the Distributor
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Distributors
    put:
      summary: This method is used to update multiple distributor records in the database.
        No {distributorid} parameters should be included.
      description: This method is used to update multiple distributor records in the
        database. no {distributorid} parameters should be included..
      operationId: Distributors_Update
      x-api-path-slug: 3dcartwebapiv1distributors-put
      parameters:
      - in: body
        name: distributors
        description: A Json or XML object containing the new distributors
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
      - Distributor
      - Records
      - In
      - Database
      - ""
      - "No"
      - Distributorid
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new distributor to the system
      description: Adds a new distributor to the system.
      operationId: Distributors_Post
      x-api-path-slug: 3dcartwebapiv1distributors-post
      parameters:
      - in: body
        name: distributor
        description: A Json or XML object containing the new distributor
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
      - Distributor
      - To
      - System
  /3dCartWebAPI/v1/Distributors/{distributorid}:
    put:
      summary: This method is used to update a single distributor record in the database.
        The {distributorid} parameter specifies which distributor to update.
      description: This method is used to update a single distributor record in the
        database. the {distributorid} parameter specifies which distributor to update..
      operationId: Distributors_Update
      x-api-path-slug: 3dcartwebapiv1distributorsdistributorid-put
      parameters:
      - in: body
        name: distributor
        description: A Json or XML object containing the new distributor
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: distributorid
        description: Distributor ID
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
      - Distributor
      - Record
      - In
      - Database
      - ""
      - Distributorid
      - Parameter
      - Specifies
      - Which
      - Distributor
      - To
      - Update
  /3dCartWebAPI/v1/Distributors/{distributorid}/Products:
    get:
      summary: Get all products from a specific distributor
      description: Get all products from a specific distributor.
      operationId: Products_GetAllProductsFromDistributor
      x-api-path-slug: 3dcartwebapiv1distributorsdistributoridproducts-get
      parameters:
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
      - in: path
        name: distributorid
        description: ID of the distributor
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
      - Distributor
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