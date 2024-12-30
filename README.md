# EcoomerceAPI
A comprehensive e-commerce backend application designed to handle core functionalities such as user management, product catalog, orders, and payments. This project is built using Java, Spring Boot, Hibernate, and MySQL, ensuring scalability and maintainability.

Features

User Management:

User authentication (sign up, log in, log out).

Role-based access control (e.g., Admin, Customer).

Product Management:

Add, update, delete, and view products.

Product categories and filtering.

Order Management:

Place, view, and track orders.

Cart functionality with multiple items.

Payment Integration:

Mock payment gateway for processing orders.

Database Management:

CRUD operations for all entities.

Relationships between users, products, and orders using Hibernate ORM.

Tech Stack

Backend

Java

Spring Boot (Rest API Development)

Hibernate (ORM Framework)

Database

MySQL

Tools & Libraries

Maven (Dependency Management)

Swagger (API Documentation)

Lombok (Boilerplate Code Reduction)

JUnit (Testing)

Prerequisites

Java 8 or later

Maven

MySQL

An IDE (e.g., IntelliJ IDEA, Eclipse) or a text editor.

Installation & Setup

Clone the Repository:

git clone https://github.com/yourusername/EcoomerceAPI.git
cd EcoomerceAPI

Set up the Database:

Create a MySQL database named ecommerce_db.

Update the application.properties file with your MySQL credentials.

spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
spring.datasource.username=your-username
spring.datasource.password=your-password

Run the Application:

mvn spring-boot:run

The application will start on http://localhost:8080.

Access the Swagger UI:
Navigate to http://localhost:8080/swagger-ui/ to explore the APIs.

Project Structure

EcoomerceAPI/
|-- src/main/java
|   |-- com.example.ecommerce
|       |-- controllers
|       |-- models
|       |-- repositories
|       |-- services
|-- src/main/resources
|   |-- application.properties
|-- pom.xml

controllers: Handle HTTP requests and map them to services.

models: Define entity classes and database schema.

repositories: Provide CRUD operations for entities.

services: Contain business logic and interact with repositories.

API Endpoints

User Endpoints

POST /users/register: Register a new user.

POST /users/login: Authenticate a user.

Product Endpoints

GET /products: Retrieve all products.

POST /products: Add a new product (Admin only).

PUT /products/{id}: Update a product (Admin only).

DELETE /products/{id}: Delete a product (Admin only).

Order Endpoints

POST /orders: Place a new order.

GET /orders: View all orders for the logged-in user.

Payment Endpoints

POST /payments: Process a payment.

Contribution

Contributions are welcome! To contribute:

Fork the repository.

Create a new branch (git checkout -b feature/your-feature-name).

Commit your changes (git commit -m 'Add some feature').

Push to the branch (git push origin feature/your-feature-name).

Open a pull request.


Author

Laraib Khan

Email: laraib8090khan@gmail.com

LinkedIn: Laraib Khan

GitHub: laraib05

