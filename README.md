
# E-Commerce Spring Boot Practice

## Overview
This project is a practice implementation of an e-commerce application using Spring Boot. It demonstrates various aspects of building a robust and scalable e-commerce application, including CRUD operations, database integration, and web development.

## Features
- **User Management**: Create, read, update, and delete user information.
- **Product Management**: Manage products, including adding new products, updating existing ones, and deleting products.
- **Order Management**: Handle customer orders, including order creation and tracking.
- **Database Integration**: Uses H2 in-memory database for persistent storage.
- **Development Tools**: Includes Spring Boot DevTools for hot swapping during development.

## Microservices
This project is composed of several microservices, each responsible for a specific domain of the application:

1. **User Service**
   - Manages user information and authentication.
   - Exposes RESTful APIs for user operations.
   - Uses Spring Data JPA for database interactions.

2. **Product Service**
   - Manages product catalog, including product details and inventory.
   - Exposes RESTful APIs for product operations.
   - Uses Spring Data JPA for database interactions.

3. **Order Service**
   - Handles order processing, including order creation and tracking.
   - Exposes RESTful APIs for order operations.
   - Uses Spring Data JPA for database interactions.

4. **API Gateway**
   - Acts as a single entry point for all client requests.
   - Routes requests to the appropriate microservices.
   - Uses Spring Cloud Gateway.

5. **Service Discovery**
   - Uses Eureka for service registration and discovery.
   - Ensures that microservices can find and communicate with each other.

## Technologies Used

### Backend
- **Spring Boot**: Framework to create stand-alone, production-grade Spring based Applications.
- **Spring Data JPA**: Abstraction over the JPA to interact with relational databases.
- **Spring Web**: Framework for building web applications, including RESTful services.
- **H2 Database**: In-memory database for development and testing.
- **Lombok**: Java library that automatically plugs into your editor and build tools, simplifying Java development.
- **Spring Cloud Gateway**: Provides a library for building an API Gateway on top of Spring WebFlux.
- **Spring Cloud Netflix Eureka**: Service registry for service discovery.

## Prerequisites
- Java 21
- Maven

## Getting Started

### Clone the repository
```bash
git clone https://github.com/GRVKMR2003/E-Commerce-Springboot-Practice.git
cd E-Commerce-Springboot-Practice/ecom-proj-master
```

### Build the project
```bash
mvn clean install
```

### Run the project
```bash
mvn spring-boot:run
```

The application will be running on `http://localhost:8080`.

## Project Structure
- **src/main/java**: Contains the main application code.
- **src/main/resources**: Contains application properties and static resources.
- **src/test/java**: Contains test cases for the application.

## Usage
- **User Management**: Manage user information through RESTful APIs.
- **Product Management**: Manage product information through RESTful APIs.
- **Order Management**: Handle customer orders through RESTful APIs.

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- Spring Boot
- Spring Data JPA
- Spring Web
- H2 Database
- Lombok
- Spring Cloud Gateway
- Spring Cloud Netflix Eureka
