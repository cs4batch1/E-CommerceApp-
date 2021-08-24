# Introduction
This is one of my E-commerce API app implementations. It is written in python, using Django and as the main frameworks.
This is not a finished project by any means, but it has a valid enough shape to be git cloned and studied if you are interested in this topic.
If you are interested in this project take a look at my other server API implementations I have made with:

- Django
- Java Spring Boot + Hibernate
- Node Js 

 The short url for comments, does not seem to work, /comments/:id does not work, but
 /products/:slug/comments/:pk does ... hum, fix it
 - Security:
    - Secure file upload
    - Secure all user input
    - CORS
- then run server with
`python3 manage.py runserver 8080`
It is convenient to use port 8080 because all the requests made in postman are using that port, the postman file is `api.postman_collection.json`,
you can import it and test the requests by yourself -)


# Features
- Authentication / Authorization
- Paging
- Products, Orders, OrderItems, Addresses, Custom User model, Tags, Categories, Comments, TimestampedModel, FileUpload(Polymorphic)
- Products associated to images, file upload without any 3party package
- CRUD operations on products, comments, tags, categories

    
        
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
```
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
