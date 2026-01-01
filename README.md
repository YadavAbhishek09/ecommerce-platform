# E-commerce Platform

## Problem Statement
Build a scalable e-commerce backend that supports product management, orders,
authentication, and role-based access.

## Architecture Overview
- Spring Boot REST API
- Layered architecture (Controller → Service → Repository)
- MySQL for persistence
- JWT-based authentication
- React frontend (separate repo / folder)

## Key Features
- Product CRUD with pagination & filtering
- Order lifecycle management
- User authentication & authorization
- Input validation & global error handling

## Data Model
Explain main entities:
- User
- Product
- Order
- OrderItem

## API Design
List main endpoints (short, not Swagger dump)

## Security
- JWT authentication
- Role-based access control

## Testing
- Unit tests for services
- Integration tests for controllers

## How to Run Locally
Step-by-step instructions

## Trade-offs & Future Improvements
- Caching
- Async order processing
- Search optimization
