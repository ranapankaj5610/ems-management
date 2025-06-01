
---

### ✅ `ems-backend/README.md`

```markdown
# EMS Backend

This is the **backend** part of the EMS (Employee Management System) project, built using **Spring Boot**, **Spring Data JPA**, and **MySQL**. It provides RESTful APIs to manage employee data.

---

## 🔧 Tech Stack

- Spring Boot
- Spring Data JPA
- MySQL
- Maven

---

## 🚀 How to Run the Backend

### ✅ Prerequisites

- Java 17+ installed
- MySQL running locally
- Maven installed (or use the provided `mvnw` script)

### 🛠️ Steps

1. **Create MySQL database**

   ```sql
   CREATE DATABASE ems;

2. Configure database in application.properties

 spring.datasource.url=jdbc:mysql://localhost:3306/ems
 spring.datasource.username=root
 spring.datasource.password=your_password
 spring.jpa.hibernate.ddl-auto=update

3. Run the application
 cd ems-backend
 ./mvnw spring-boot:run

4. App will be running at:
 http://localhost:8080

🌐 API Endpoints
 | Method | Endpoint              | Description         |
| ------ | --------------------- | ------------------- |
| GET    | `/api/employees`      | Fetch all employees |
| POST   | `/api/employees`      | Add a new employee  |
| GET    | `/api/employees/{id}` | Get employee by ID  |
| PUT    | `/api/employees/{id}` | Update employee     |
| DELETE | `/api/employees/{id}` | Delete employee     |
