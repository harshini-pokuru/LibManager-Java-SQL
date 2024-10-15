# LibManager

## Project Overview
The Library Management System is a Java-based application built using Swing for the graphical user interface (GUI) and MySQL for the backend database. The system is designed to manage daily library operations such as book inventory, staff management, and administrative tasks. The goal is to provide a simple, efficient, and secure solution for library administrators.

## Key Features
- **User Authentication**: Secure login for administrative access.
- **Dashboard**: A central interface for managing books, staff, and admin settings.
- **Book Management**: Add, view, and remove books from the library's catalog.
- **Staff Management**: Add, view, and remove staff members from the system.
- **Admin Management**: Edit admin credentials for secure access.

## Technologies Used
- **Java**: Core language used for the application logic and Swing GUI.
- **Swing**: Used for the graphical user interface.
- **MySQL**: Backend database for storing information about books, staff, and admin users.
- **JDBC**: Java Database Connectivity used for database interaction.

## Project Components

### 1. Login Page
- **Purpose**: Authenticates admin users.
- **Technology**: Java Swing form with JDBC for database verification.

### 2. Dashboard
- **Purpose**: Central navigation hub for library operations.
- **Components**: Buttons for Book Management, Staff Management, Admin Settings.

### 3. Book Management
- **Add Books**: Input form to add new books to the library.
- **View Books**: Display all available books from the database in a table.
- **Remove Books**: Select and remove books from the catalog.

### 4. Staff Management
- **Add Staff**: Input form to add new staff members.
- **View Staff**: Display staff details in a table.
- **Remove Staff**: Remove staff from the system based on their details.

### 5. Admin Settings
- **Edit Admin Credentials**: Allows the admin to change username or password securely.

## Database Schema
The application uses a simple database schema for storing information about books, staff, and admin users.

### Tables
1. **Books Table**: Stores book details like `book_id`, `title`, `author`, and `genre`.
2. **Staff Table**: Stores staff details like `staff_id`, `name`, and `role`.
3. **Admin Table**: Stores admin credentials like `admin_id`, `username`, and `password`.

## Security Considerations
- **Password Storage**: Admin passwords should be hashed before storage.
- **Input Validation**: Ensure input validation to prevent SQL injection.

## Potential Enhancements
- **User Roles**: Although this system is designed as an admin-centric interface, future versions could introduce varied access levels, such as limited access for support staff, but still keeping the primary control with the admin.
- **Search Functionality**: Implement advanced search options for administrators to quickly find books or staff members using filters such as title, author, or staff name.
