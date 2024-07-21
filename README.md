Node.js Microservices Project

Overview

This project is a Node.js-based microservices architecture consisting of three main services: Customer, Shopping, and Product. Each service operates independently, ensuring modularity, scalability, and ease of maintenance. The system is designed with modern best practices, including RESTful APIs, asynchronous messaging with RabbitMQ, MongoDB for data storage, JWT-based authentication, and automated CI/CD pipelines.
Table of Contents

    Features
    Architecture
    Services
        Customer Service
        Shopping Service
        Product Service
    Getting Started
        Prerequisites
        Installation
    Usage
    Testing
    Deployment
    Documentation
    Contributing
    License

Features

    Scalable Microservices Architecture: Independent customer, shopping, and product services.
    RESTful APIs: Efficient data exchange and integration.
    Asynchronous Messaging with RabbitMQ: Reliable inter-service communication.
    MongoDB Databases: High data consistency and availability.
    JWT-based Authentication: Secure authentication and authorization.
    Automated CI/CD Pipelines: Streamlined testing, integration, and deployment.
    Containerization with Docker: Consistent and efficient local development.
    Service Orchestration with Kubernetes: Seamless service discovery, load balancing, and scaling.
    Comprehensive Testing with Jest: High code coverage and reliability.
    Centralized Error Handling and Logging: Improved system robustness.
    Thorough Documentation: Facilitates onboarding and knowledge transfer.

Architecture

The project employs a microservices architecture with the following services:

    Customer Service: Manages customer-related operations.
    Shopping Service: Handles shopping cart and order management.
    Product Service: Manages product-related operations.

Each service is built with Node.js and Express, uses MongoDB for data storage, and communicates asynchronously through RabbitMQ.
Services
Customer Service

    API Endpoints:
        GET /customers: Retrieve customer information.
        POST /customers: Create a new customer.
    Source Code: Located in the /customer directory.
    Key Files:
        src/express-app.js: Express server setup.
        src/api/customer.js: Customer-related endpoints.
        src/database/models/Customer.js: Customer model.

Shopping Service

    API Endpoints:
        GET /shopping/cart: Retrieve shopping cart information.
        POST /shopping/order: Create a new order.
    Source Code: Located in the /shopping directory.
    Key Files:
        src/express-app.js: Express server setup.
        src/api/shopping.js: Shopping-related endpoints.
        src/database/models/Cart.js: Cart model.
        src/database/models/Order.js: Order model.

Product Service

    API Endpoints:
        GET /products: Retrieve product information.
        POST /products: Create a new product.
    Source Code: Located in the /product directory.
    Key Files:
        src/express-app.js: Express server setup.
        src/api/product.js: Product-related endpoints.
        src/database/models/Product.js: Product model.