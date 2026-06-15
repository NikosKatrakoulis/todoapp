# 📝 Todo Application

A simple Todo web application built with **Spring Boot**, **MySQL** and **Thymeleaf**.

## 🚀 Features

- View all tasks
- Add new tasks
- Toggle task completion status
- Delete tasks

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Java 21, Spring Boot 4.1.0 |
| ORM | Spring Data JPA, Hibernate |
| Frontend | Thymeleaf, Bootstrap 5 |
| Database | MySQL 9.x |
| Build Tool | Maven |
| Other | Lombok |

## ⚙️ Prerequisites

- Java 21+
- MySQL 8.x or 9.x
- Maven

## 🔧 Setup & Installation

### 1. Clone the repository

```bash
git clone https://github.com/NikosKatrakoulis/todoapp.git
cd todoapp
```

### 2. Create the MySQL database

```sql
CREATE DATABASE `todo-app`;
```

### 3. Configure application properties

Create the file `src/main/resources/application.properties` with your database credentials:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/todo-app
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
```

### 4. Run the application

```bash
./mvnw spring-boot:run
```

### 5. Open in browser

```
http://localhost:8080/tasks
```

## 📁 Project Structure

```
src/
├── main/
│   ├── java/com/app/todoapp/
│   │   ├── controller/     # TaskController
│   │   ├── models/         # Task entity
│   │   ├── repository/     # TaskRepository
│   │   └── services/       # TaskService
│   └── resources/
│       └── templates/      # Thymeleaf HTML templates
```

## 👤 Author

**Nikos Katrakoulis**  
GitHub: [@NikosKatrakoulis](https://github.com/NikosKatrakoulis)