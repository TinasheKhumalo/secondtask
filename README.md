I am GPT-5.

# First REST API with Spring Boot

A beginner-friendly RESTful API built with Java and Spring Boot. This project demonstrates the fundamentals of REST architecture and provides basic CRUD operations on a product catalog. It is intended to help you quickly understand how to create, run, and test a REST API using Spring Boot.

## ✅ Features
- Create new products
- Retrieve one or all products
- Update existing products
- Delete products
- Uses H2 in-memory database for easy testing
- Simple to test with Postman or curl

## 🛠 Technologies
- Java 17+
- Spring Boot
- Maven (with wrapper)
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

## 🚀 Get started (you)
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd first-rest-api-java-master
   ```
   Replace `<repository-url>` with the actual repository URL.

2. Run the application:
   - On macOS/Linux:
     ```bash
     ./mvnw spring-boot:run
     ```
   - On Windows:
     ```bash
     mvnw.cmd spring-boot:run
     ```
   Or run the app from your IDE by launching `FirstRestApiApplication.java`.

3. The server starts on:
   ```
   http://localhost:8080
   ```

## 🔗 API Endpoints
| Method | Endpoint           | Description             |
|--------|--------------------|-------------------------|
| GET    | /products          | Get all products        |
| GET    | /products/{id}     | Get product by ID       |
| POST   | /products          | Create a new product    |
| PUT    | /products/{id}     | Update existing product |
| DELETE | /products/{id}     | Delete a product        |

Example curl requests:
- Create:
  ```bash
  curl -X POST http://localhost:8080/products \
    -H "Content-Type: application/json" \
    -d '{"name":"Widget","price":9.99,"description":"A sample product"}'
  ```
- Get all:
  ```bash
  curl http://localhost:8080/products
  ```
- Get by id:
  ```bash
  curl http://localhost:8080/products/1
  ```
- Update:
  ```bash
  curl -X PUT http://localhost:8080/products/1 \
    -H "Content-Type: application/json" \
    -d '{"name":"Updated Widget","price":11.99,"description":"Updated"}'
  ```
- Delete:
  ```bash
  curl -X DELETE http://localhost:8080/products/1
  ```

## 🗃 H2 Console (in-memory DB)
You can access the H2 console while the app is running:
```
http://localhost:8080/h2-console
```
- JDBC URL: `jdbc:h2:mem:testdb`  
- Username: `sa`  
- Password: (leave blank)

## 📸 Screenshots
(Replace the links below with your image paths in the repo)
- PUT request screenshot: ![put](path/to/put.png)
- POST request screenshot: ![post](path/to/post.png)
- GET all screenshot: ![get-all](path/to/get-all.png)
- GET by id screenshot: ![get](path/to/get.png)
- DELETE screenshot: ![delete](path/to/delete.png)
- H2 database screenshot: ![database](path/to/database.png)

## 📄 License
This project is licensed under the MIT License. You are free to use, modify, and distribute the code.

---

If you want, I can:
- Add a ready-to-use .gitignore,
- Create a CONTRIBUTING.md,
- Add example Postman collection or GitHub Actions CI workflow,
- Or adapt this README to include badges and more detailed examples.

Which would you like me to add before you upload?
