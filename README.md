# E-commerce Backend Service

Backend service for an e-commerce platform built using **Java and Spring Boot**.
The application exposes REST APIs to manage products, including creation,
retrieval, update, deletion, image handling, and search functionality.

This project focuses on clean REST API design, layered architecture,
and backend engineering fundamentals.

---

## Problem Statement

Design and implement a backend system for an e-commerce application that supports:
- Product management (CRUD)
- Product image upload and retrieval
- Search functionality
- Scalable and maintainable API design

---

## Tech Stack

- **Backend:** Java, Spring Boot
- **Web:** Spring MVC (REST APIs)
- **Persistence:** JPA / Hibernate
- **Database:** MySQL / PostgreSQL (configurable)
- **File Handling:** Multipart file upload
- **Build Tool:** Maven
- **Frontend:** React (separate module/repository)

---

## Architecture Overview

Controller - Service - Repository - Database 


- **Controller Layer:** Handles HTTP requests and responses
- **Service Layer:** Contains business logic
- **Repository Layer:** Handles database interactions using JPA
- **Model Layer:** Defines domain entities

This separation improves testability, maintainability, and scalability.

---

## Core Features

### Product Management
- Fetch all products
- Fetch product by ID
- Create new product with image upload
- Update existing product and image
- Delete product

### Image Handling
- Supports multipart image upload
- Retrieves product image by product ID

### Search
- Keyword-based product search across multiple fields

---

## API Endpoints (High-Level)

| Method | Endpoint | Description |
|------|---------|-------------|
| GET | `/api/products` | Get all products |
| GET | `/api/product/{id}` | Get product by ID |
| POST | `/api/product` | Add new product with image |
| PUT | `/api/product/{id}` | Update product |
| DELETE | `/api/product/{id}` | Delete product |
| GET | `/api/product/{id}/image` | Get product image |
| GET | `/api/products/search?keyword=` | Search products |

---

## Data Model (Simplified)

**Product**
- id
- name
- description
- brand
- price
- category
- releaseDate
- available
- stock
- image (byte[])

---

## Error Handling

- Uses HTTP status codes to indicate success or failure
- Returns `404` for resource not found
- Returns `500` for server errors

> Planned improvement: Centralized exception handling using `@ControllerAdvice`

---

## How to Run Locally

1. Clone the repository
2. Configure database credentials in `application.properties`
3. Run the Spring Boot application
4. Access APIs at `http://localhost:8080/api`

---

## Future Improvements

- Add pagination and sorting
- Introduce DTOs to avoid exposing entities directly
- Centralized exception handling
- Validation using `@Valid`
- Unit and integration tests
- Authentication and authorization (JWT)
- Dockerization
- API documentation using Swagger/OpenAPI

---

## Author

**Abhishek Yadav**  
Java Backend / Full-Stack Engineer


