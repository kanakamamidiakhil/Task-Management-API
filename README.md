# Task Management API

##  How to Install & Run the Project

### 1. Prerequisites

Ensure the following are installed on your system:

| Requirement        | Minimum Version | Download Link                                                                  |
| ------------------ | --------------- | ------------------------------------------------------------------------------ |
| **Java JDK**       | 17+             | [https://adoptium.net/](https://adoptium.net/)                                 |
| **Maven**          | 3.8+            | [https://maven.apache.org/download.cgi](https://maven.apache.org/download.cgi) |
| **PostgreSQL**     | 13+             | [https://www.postgresql.org/download/](https://www.postgresql.org/download/)   |
| **Git** (Optional) | Latest          | [https://git-scm.com/downloads](https://git-scm.com/downloads)                 |

---

### 2. Clone the Project

```bash
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
```

---

### 3. Setup PostgreSQL Database

1. Open PostgreSQL (pgAdmin/CLI)
2. Create a Database:

```sql
CREATE DATABASE your_database_name;
```

3. Update your database credentials in **application.properties**:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/your_database_name
spring.datasource.username=postgres
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
```

---

### 4. Install Dependencies

Run Maven install to download all required dependencies:

```bash
mvn clean install
```

> Maven will automatically install all dependencies specified in the `pom.xml`.

---

### 5. Run the Application

```bash
mvn spring-boot:run
```

OR run the main class from your IDE.

---

### 6. Access the Application

Default URL:

```
http://localhost:8080
```

---

---



