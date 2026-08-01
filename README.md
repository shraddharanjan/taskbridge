# 🛠️ TaskBridge

TaskBridge is a full-stack task marketplace inspired by platforms such as Airtasker. It connects people who need help completing everyday tasks with local taskers looking for work.

The application supports two account types:

- **Posters** can create and manage tasks, set budgets and locations, and review applicants.
- **Taskers** can browse opportunities, filter and save tasks, apply for work, and maintain a profile with a CV.

The project was built with **Java 21**, **Spring Boot**, **Thymeleaf**, **Spring Security**, **JPA/Hibernate**, and **MySQL**.

> **Live demo:**
> https://taskbridge-ijyj.onrender.com/

---

## ✨ Features

### Authentication and accounts

- Secure registration and login using Spring Security
- BCrypt password hashing
- Role-based access for Poster and Tasker accounts
- Separate profile and dashboard experiences for each account type

### Poster features

- Create task listings with a title, description, budget, location, work type, and work arrangement
- View and manage posted tasks
- Edit or delete existing tasks
- Review the taskers who have applied
- Open applicant profiles and download submitted CVs

### Tasker features

- Browse available tasks
- Search by task title and location
- Filter opportunities by employment type, location arrangement, and date posted
- Save tasks for later
- Apply to multiple different tasks
- Upload a profile photo and CV
- View previously saved and applied-for tasks

### Application features

- Responsive Thymeleaf user interface
- Role-based navigation and protected routes
- Persistent MySQL storage through Spring Data JPA and Hibernate
- Rich-text task descriptions using Summernote
- File upload support for profile photographs and CVs
- Composite database constraints that prevent duplicate applications to the same task

---

## ⚙️ Tech Stack

| Technology | Purpose |
|---|---|
| **Java 21** | Primary programming language |
| **Spring Boot 3** | Application framework and embedded web server |
| **Spring MVC** | Controllers, routing, and form handling |
| **Spring Security** | Authentication, password hashing, and role-based authorization |
| **Thymeleaf** | Server-side HTML rendering |
| **Spring Data JPA** | Repository and persistence layer |
| **Hibernate** | Object-relational mapping and schema integration |
| **MySQL** | Relational database |
| **Bootstrap** | Responsive layout utilities and components |
| **HTML / CSS / JavaScript** | Frontend structure, styling, and interactions |
| **Summernote** | Rich-text task description editor |
| **Maven** | Dependency management and build tooling |
| **Docker** | Production deployment packaging |
| **Render** | Planned application hosting |
| **Aiven** | Hosted MySQL database |

---

## 🏗️ Project Structure

```text
src/
├── main/
│   ├── java/com/shraddha/taskbridge/
│   │   ├── config/       # Security and application configuration
│   │   ├── controller/   # MVC controllers and routes
│   │   ├── entity/       # JPA entities
│   │   ├── repository/   # Spring Data repositories
│   │   └── services/     # Business logic and service classes
│   └── resources/
│       ├── static/       # CSS, JavaScript, images, and other assets
│       ├── templates/    # Thymeleaf templates
│       └── application.properties
├── test/
pom.xml
mvnw
mvnw.cmd
```

---


## 🧪 Suggested Test Flow

Before deploying a new version, test that:

1. A Poster can register and log in.
2. A Tasker can register and log in.
3. A Poster can create, edit, and delete a task.
4. A Tasker can browse, save, and apply for tasks.
5. A Tasker can apply to multiple different tasks.
6. A Poster can view applicants for their own tasks.
7. Profile photo and CV upload validation works.
8. Role-protected pages cannot be opened by the wrong account type.
9. Logout clears the user session.

---

## 🔭 Future Improvements

- Move user uploads to persistent cloud storage
- Add email verification and password reset
- Add task categories and richer search filters
- Add messaging between Posters and Taskers
- Add application status tracking
- Add automated unit and integration tests
- Add Flyway or Liquibase database migrations
- Add CI/CD checks with GitHub Actions
- Add pagination for large task lists

---

## 👩‍💻 Author

**Shraddha Ranjan**

Built as a full-stack Java and Spring Boot portfolio project.
