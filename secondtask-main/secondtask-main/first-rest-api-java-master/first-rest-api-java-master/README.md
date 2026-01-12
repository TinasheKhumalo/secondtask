# First REST API with Spring Boot

This project is a beginner-friendly RESTful API built with **Java** and **Spring Boot**. It demonstrates the fundamental principles of REST architecture and provides basic CRUD operations on a product catalog. The goal of this project is to help newcomers understand how to create and manage REST APIs in a clean, structured manner using Spring Boot.

## 📦 Features

- ✅ Create new products
- 🔍 Retrieve single or multiple products
- ✏️ Update existing products
- ❌ Delete products
- 💾 Uses H2 in-memory database
- 🧪 Easy to test with tools like Postman or curl

## 🛠 Technologies Used

- Java 17+
- Spring Boot
- Maven
- H2 Database
- Spring Web

## 📁 Project Structure

```
src/
└── main/
    └── java/com/springstarter/first_rest_api/
        ├── FirstRestApiApplication.java
        └── product/
            ├── api/
            │   ├── ProductController.java
            │   ├── request/
            │   │   ├── ProductRequest.java
            │   │   └── UpdateProductRequest.java
            │   └── response/
            │       └── ProductResponse.java
            ├── domain/
            │   └── Product.java
            └── repository/
                └── ProductRespository.java
```

## 🚀 Getting Started

### Prerequisites

Ensure the following tools are installed:

- Java 17 or higher
- Maven

### Run the Application

```bash
git clone <repository-url>
cd first-rest-api-java-master
./mvnw spring-boot:run
```

The server will start at `http://localhost:8080`.

## 🔗 API Endpoints

| Method | Endpoint           | Description             |
|--------|--------------------|-------------------------|
| GET    | /products          | Get all products        |
| GET    | /products/{id}     | Get product by ID       |
| POST   | /products          | Create a new product    |
| PUT    | /products/{id}     | Update existing product |
| DELETE | /products/{id}     | Delete a product        |

## 🗃 Database Access (H2 Console)

The application uses an H2 in-memory database. You can access the H2 console at:

```
http://localhost:8080/h2-console
```

**JDBC URL:** `jdbc:h2:mem:testdb`  
**Username:** `sa`  
**Password:** *(leave blank)*

## 📸 Screenshots

-![put](https://github.com/user-attachments/assets/c66c076a-3236-44a8-a586-620057826c3f)
![post](https://github.com/user-attachments/assets/3ff00d43-402b-423c-9e7e-f1570a21a147)
![get-all](https://github.com/user-attachments/assets/ada0d031-ab43-484a-908f-0388b6fd2ed1)
![get](https://github.com/user-attachments/assets/0e995323-068c-457b-8035-d3381f26a52c)
![delete](https://github.com/user-attachments/assets/15ce1df1-fe13-4d81-b06c-18a16029d7f3)
![database](https://github.com/user-attachments/assets/e98f9e9f-6177-41bb-9f65-d945f9b0e177)





## 📄 License

This project is licensed under the MIT License. You are free to use, modify, and distribute this code as needed.

---

Happy Coding! 🎉
