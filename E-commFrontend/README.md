# E-commerce Frontend Application

Frontend application for an e-commerce platform built using **React**.
This application consumes REST APIs exposed by the Spring Boot backend
to manage products, display product listings, and handle user interactions.

The focus of this project is clean UI architecture, API integration,
and separation of frontend and backend responsibilities.

---

## Overview

This frontend application provides a user interface for:
- Viewing product listings
- Searching products
- Viewing product details
- Adding and updating products (admin functionality)
- Displaying product images served by the backend

The frontend is designed to be **backend-agnostic** and communicates
with the backend exclusively via REST APIs.

---

## Tech Stack

- **Frontend Framework:** React
- **Language:** JavaScript
- **State Management:** React Hooks
- **HTTP Client:** Axios / Fetch API
- **Styling:** CSS / Bootstrap (if used)
- **Build Tool:** npm / Vite / Create React App

---

## Application Architecture
components/
├── ProductList
├── ProductCard
├── ProductDetails
├── ProductForm
└── SearchBar

services/
└── productService.js

pages/
├── Home
├── ProductDetails
└── Admin


### Key Design Principles
- Reusable UI components
- Separation of UI and API logic
- Stateless components where possible
- Centralized API communication

---

## Features

### Product Listing
- Displays all available products
- Shows product name, price, brand, and availability

### Product Search
- Keyword-based search
- Real-time filtering using backend search API

### Product Details
- Detailed view of a selected product
- Displays product image fetched from backend

### Product Management (Admin)
- Add new product with image upload
- Update existing product details
- Delete products

---

## Backend Integration

The frontend integrates with the Spring Boot backend using REST APIs.

### Example API Calls
- `GET /api/products`
- `GET /api/product/{id}`
- `POST /api/product`
- `PUT /api/product/{id}`
- `DELETE /api/product/{id}`
- `GET /api/product/{id}/image`

API base URL is configurable via environment variables.

---

## Environment Configuration

Create a `.env` file in the root directory:


This allows seamless switching between local and deployed backends.

---

## How to Run Locally

1. Clone the repository
2. Install dependencies: npm install
3. Start the application: npm start
4. 4. Open browser at: http://localhost:3000

---

## Error Handling

- Graceful handling of API failures
- User-friendly error messages
- Fallback UI for network issues

---

## Future Improvements

- Client-side pagination
- Authentication and role-based UI
- Improved form validation
- Loading and skeleton states
- Performance optimization
- Unit tests for components
- Integration tests with mocked APIs

---

## Project Structure Goals

This frontend is intentionally kept:
- Simple
- Readable
- Easy to extend

Complex business logic is handled by the backend to keep the UI lightweight.

---

## Author

**Abhishek Yadav**  
Java Backend / Full-Stack Engineer
