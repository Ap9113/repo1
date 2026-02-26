# Spring Boot REST API Example

This project demonstrates a simple RESTful API built with Spring Boot, Spring Data JPA, H2 in-memory database, and Lombok.

## Features
- CRUD operations for a `User` entity
- Exception handling with custom exceptions and global handler
- Validation using Bean Validation (Hibernate Validator)
- In-memory H2 database for easy testing
- Dockerfile for containerization

## Requirements
- Java 17+
- Maven 3.6+
- Docker (optional)

## Getting Started

1. Clone the repo:

   ```bash
   git clone https://github.com/yourusername/springboot-rest-api.git
   cd springboot-rest-api
   ```

2. Build and run with Maven:

   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

3. The API will be available at `http://localhost:8080/api/users`.

4. To run with Docker:

   ```bash
   docker build -t springboot-rest-api .
   docker run -p 8080:8080 springboot-rest-api
   ```

## API Endpoints

| Method | URL                | Description           |
|--------|--------------------|-----------------------|
| GET    | /api/users         | Get all users         |
| GET    | /api/users/{id}    | Get user by ID        |
| POST   | /api/users         | Create new user       |
| PUT    | /api/users/{id}    | Update existing user  |
| DELETE | /api/users/{id}    | Delete user by ID     |

## Sample JSON

```json
{
  "firstName": "John",
  "lastName": "Doe",
  "email": "john.doe@example.com"
}
```

## License
MIT License
