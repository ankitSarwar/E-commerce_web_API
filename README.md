<h1 align = "center"> E-commerce web_API </h1>

<p align="center">
<a href="Java url">
    <img alt="Java" src="https://img.shields.io/badge/Java->=8-darkblue.svg" />
</a>
<a href="Maven url" >
    <img alt="Maven" src="https://img.shields.io/badge/maven-3.0.5-brightgreen.svg" />
</a>
<a href="Spring Boot url" >
    <img alt="Spring Boot" src="https://img.shields.io/badge/Spring Boot-3.0.6-brightgreen.svg" />
</a>
<a >
    <img alt="MySQL" src="https://img.shields.io/badge/MySQL-blue.svg">
</a>
</p>

This is a simple E-Commerce WebApp built using Spring Boot, Spring Security, and Hibernate. 
The application allows users to view product categories, products, place orders, and manage user accounts.
It includes authentication and authorization mechanisms to control access to different endpoints based on user roles.

---

## Framework Used
* Spring Boot
---

## Dependencies
The following dependencies are required to run the project:

* Spring Boot Dev Tools
* Spring Web
* Spring Data JPA
* MySQL Driver
* Lombok
* Validation
* Swagger

<br>

>## Features

 * User Registration and Authentication: Users can create accounts by registering with the application. The authentication process ensures that only registered users can access restricted endpoints.

* Role-Based Access Control: The application supports role-based access control, with two main roles: "ROLE_USER" and "ROLE_ADMIN." Certain endpoints are accessible only to users with specific roles.

* Product Management: Admin users have the ability to add new product categories and individual products. Products are associated with specific categories to facilitate easy browsing.

* Order Placement: Authenticated users can place orders for products they wish to purchase. The application records order details, including product quantity, user information, and shipping address.

* Address Management: Users can manage their shipping addresses, allowing them to select the desired address during the order placement process.


>## API Endpoints
>GET /order/getAllCategory: Get all product categories.

>POST /user/new: Register a new user.

>POST /user/authenticate: Authenticate a user and get the JWT token.
>
>DELETE /user/{id}: Delete a user (requires admin role).
>
>GET /admin/products: Get all products (requires admin role).
>
>POST /admin/addCategory: Add a new product category (requires admin role).
>
>POST /admin/addProduct: Add a new product (requires admin role).
>
>POST /user/address: Add a new address.
>
>POST /order/placeOrder: Place a new order.
>
>GET /order: Get all orders (requires user role).

---
## Security
  The application uses JWT (JSON Web Tokens) for authentication. 
  Users need to authenticate using their credentials to access certain endpoints. The JWT token is included in the request header for authentication.


## Project Summary
  The E-Commerce WebApp is a comprehensive web application developed using Java and the Spring framework.
  It aims to provide users with a seamless online shopping experience by offering a range of features.
  The application allows users to register, sign in, and manage their profile information effectively. 
  Additionally, users can explore and purchase products from various categories, and place orders securely.
