# Library Management System - Microservices Architecture

This project is a **Library Management System** built using a microservices architecture. The system is designed to efficiently handle the core functionalities of a library, with each service dedicated to a specific responsibility. The frontend is implemented in **TypeScript** for a seamless user interface.

## Microservices Overview

The system consists of the following four microservices:

1. **User Service**  
   Manages user registrations, authentication, and user details.  
   - User creation and login
   - Profile management and user permissions

2. **Book Service**  
   Manages the library's book collection, including adding, updating, and searching books.  
   - Add new books
   - Search and list available books
   - Manage book stock and availability

3. **Borrowing Service**  
   Handles borrowing transactions, including loaning books to users and tracking due dates.  
   - Borrow a book
   - Track due dates and overdue books
   - Return books and update book status

4. **Review Service**  
   Allows users to submit and view reviews for books.  
   - Submit reviews for books
   - View all reviews for a book
   - Rate and comment on books

## Frontend Overview

The frontend is built using **TypeScript** and is designed to interact with the backend services.

## Technologies Used

### Backend:
- **Node.js** (for microservices)
- **Database**: MySQL 
- **API Communication**: RESTful APIs

### Frontend:
- **TypeScript**

### Miscellaneous:
- **Docker**: For containerization of services

## Features

- **User Service**: Handle user authentication and profile management.
- **Book Service**: Manage library books, search for available books, and view details.
- **Borrowing Service**: Loan books to users, track due dates, and handle returns.
- **Review Service**: Allow users to review and rate books.
- **Frontend**: A TypeScript-based UI that interacts with the backend services.


