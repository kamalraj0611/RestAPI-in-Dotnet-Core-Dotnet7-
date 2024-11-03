# RestAPI in .NET Core (.NET 7)

This repository hosts a REST API project built using .NET Core and .NET 7. It serves as a practical example for implementing CRUD operations, authorization, validation, and dependency injection in a clean, scalable, and maintainable way. The project demonstrates best practices in API development and is structured to support extensibility and ease of testing.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [API Documentation](#api-documentation)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Features

- RESTful API following best practices
- CRUD (Create, Read, Update, Delete) operations for resources
- Secure authentication and authorization with JWT
- Data validation and error handling
- Dependency Injection (DI) for loose coupling and testability
- Extensible and maintainable code architecture

## Getting Started

These instructions will guide you through setting up and running the project on your local machine for development and testing purposes.

### Prerequisites

- [.NET SDK 7.x](https://dotnet.microsoft.com/download/dotnet/7.0) - .NET SDK to build and run the application
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) - SQL Server for database management
- [Postman](https://www.postman.com/downloads/) - for testing the API endpoints

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/kamalraj0611/RestAPI-in-Dotnet-Core-Dotnet7-.git
    cd RestAPI-in-Dotnet-Core-Dotnet7-
    ```

2. Restore dependencies:
    ```bash
    dotnet restore
    ```

3. Set up the database:
    - Configure your connection string in `appsettings.json`.
    - Run migrations to set up the database schema.

    ```bash
    dotnet ef database update
    ```

4. Build the application:
    ```bash
    dotnet build
    ```

### Running the Application

1. Start the application:
    ```bash
    dotnet run
    ```

2. The API will be available at `http://localhost:5000`.

### API Documentation

Use Swagger to explore and test the API endpoints. After running the application, navigate to:
```
http://localhost:5000/swagger
```

### Project Structure

This project follows a clean architecture structure:

- **Controllers** - Handle HTTP requests and responses
- **Models** - Define the data structures
- **Repositories** - Manage data access and database interactions
- **Services** - Encapsulate business logic
- **DTOs** - Data Transfer Objects for cleaner and safer data transmission

### Technologies Used

- **.NET Core 7** - Core framework for building the API
- **Entity Framework Core** - ORM for database operations
- **SQL Server** - Database management system
- **Swagger** - For API documentation
- **JWT** - For secure user authentication

### Contributing

Contributions are welcome! To get started:

1. Fork the repository.
2. Create a new branch for your feature.
3. Commit your changes.
4. Open a pull request describing your changes.

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
