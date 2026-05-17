# Smart Citizen Application

A full-stack Java web application built using Spring Boot, REST APIs, and PostgreSQL — designed to manage citizen data with complete CRUD operations, a layered MVC architecture, and comprehensive backend validation.

---

## Features

- REST web services built with Spring Boot and Spring REST
- Full CRUD operations on citizen records via JDBC and PostgreSQL
- MVC architecture separating presentation, service, and data layers
- Unit testing with JUnit and Mockito for backend validation
- SLF4J logging and code coverage implementation
- Responsive UI following component design specifications

---

## Tech Stack

| Layer | Technology |
|---|---|
| Backend | Java, Spring Boot, Spring MVC, Spring REST |
| Database | PostgreSQL, JDBC |
| Testing | JUnit, Mockito, SLF4J |
| Tools | Eclipse, Git, Postman |

---

## Project Structure

```
smart-citizen-Application/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── controller/       # Spring MVC controllers (presentation layer)
│   │   │   ├── service/          # Business logic layer
│   │   │   ├── repository/       # JDBC database access
│   │   │   └── model/            # Entity classes
│   │   └── resources/
│   │       └── application.properties
│   └── test/
│       └── java/                 # JUnit + Mockito test cases
└── pom.xml
```

---

## How to Run

**Prerequisites:** Java 17+, PostgreSQL, Maven

```bash
# Clone the repository
git clone https://github.com/cheelaakhil/smart-citizen-Application.git
cd smart-citizen-Application

# Configure database
# Edit src/main/resources/application.properties:
# spring.datasource.url=jdbc:postgresql://localhost:5432/smartcitizen
# spring.datasource.username=your_username
# spring.datasource.password=your_password

# Build and run
mvn spring-boot:run
```

App runs at `http://localhost:8080`

---

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/citizens` | Get all citizens |
| GET | `/api/citizens/{id}` | Get citizen by ID |
| POST | `/api/citizens` | Create new citizen |
| PUT | `/api/citizens/{id}` | Update citizen |
| DELETE | `/api/citizens/{id}` | Delete citizen |

---

## Author

**Cheela Akhil** — [LinkedIn](https://linkedin.com/in/cheelaakhil) · [GitHub](https://github.com/cheelaakhil)
