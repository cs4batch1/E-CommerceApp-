# Introduction
This is one of my E-commerce API app implementations. It is written in python, using Django and data entry in REST API frameworks.

- Django
- Node Js 
- REST API
 

# Features
- CRUD operations on customers, products, comments, tags, categories
- Authentication / Authorization
- Products, Orders, OrderItems, Addresses, Custom User model, Tags, Categories, Comments, TimestampedModel, FileUpload(Polymorphic)
   
        
## API Endpoints
## User Routes
### * Create User

`POST |  /api/v1/users/register` 
### * Login User
`POST |  /api/v1/users/login` 

### * Get Users
`GET |  /api/v1/users` 
### * Get Single Users
`GET |  /api/v1/users/{id}` 
### * Delete User
`DELETE |  /api/v1/users/{id}` 
### * Get Users Count
`GET |  /api/v1/users/get/count` 
## Category Routes
### * Create Category
`POST |  /api/v1/categories` 

### * Get Categories
`GET |  /api/v1/categories` 
### * Get Single Category
`GET |  /api/v1/categories/{id}` 
### * Update Category
`PUT |  /api/v1/categories/{id}` 

### * Delete Category
`DELETE |  /api/v1/categories/{id}`
## Product Routes
### * Create Product
`POST |  /api/v1/products`

### * Get Products
`GET |  /api/v1/products` 
###  * Get Single Category
`GET |  /api/v1/products/{id}` 
###  * Get Prodcut Counts
`GET |  /api/v1/products/get/count` 
###  * Get Featured Prodcut Counts
`GET |  /api/v1/products/get/featured/{count}`

### * Delete Product
`DELETE |  /api/v1/products/{id}`
## Orders Routes
### * Create Order
`POST |  /api/v1/orders` 

### * Get Orders
`GET |  /api/v1/orders` 
### * Get Single Order
`GET |  /api/v1/orders/{id}` 
### * Get Total Order Count
`GET |  /api/v1/orders/get/count`
### * Get Total Sales
`GET |  /api/v1/orders/get/totalsales`
### * Get User Order
`GET |  /api/v1/orders/get/usersorders/{userid}`
### * Update Single Order
`PUT |  /api/v1/orders/{id}` 
### * Delete Single Order
`DELETE |  /api/v1/orders/{id}` 
