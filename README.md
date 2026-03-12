# Employee Management System (EMS)

A backend REST API built using Java Spring Boot and MySQL to manage employee records.

## Features

- Add new employees
- View employee list
- Update employee details
- Delete employee records

## Tech Stack

Backend:
- Java
- Spring Boot
- Spring Data JPA

Database:
- MySQL

Build Tool:
- Maven

Testing:
- Postman

## Architecture

The project follows MVC architecture:

Controller Layer
Handles API requests and responses.

Service Layer
Contains business logic.

Repository Layer
Handles database operations using Spring Data JPA.

## API Endpoints

Create Employee

POST /employees

Get All Employees

GET /employees

Get Employee By ID

GET /employees/{id}

Update Employee

PUT /employees/{id}

Delete Employee

DELETE /employees/{id}

## Database Configuration

Configured in application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/ems
spring.datasource.username=root
spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update

## How to Run

1. Clone repository
2. Open project in Spring Tool Suite
3. Run Spring Boot application
4. Test APIs using Postman

Error Handling

If an employee is not found, the API returns a custom error message:

{
  "error": "Employee not found with id: 10"
}

## Learning Outcomes

- Built REST APIs using Spring Boot
- Implemented CRUD operations
- Integrated MySQL database
- Applied MVC architecture
- Tested APIs using Postman
