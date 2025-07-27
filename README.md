# 📄 JobApk — Spring Boot Job Portal Web App

JobApk is a full-stack web application built using Spring Boot and JSP for managing and displaying job listings. It allows users to post new openings, browse available positions, and view technology stacks associated with each role — all via a responsive Bootstrap interface.

---

## 🚀 Features

- 🧾 Add new job listings with multiple tech stack options
- 📋 View all jobs in a structured, card-based format
- 📚 Store and manage job posts in-memory using Java Collections
- ✨ Responsive and interactive UI built with Bootstrap 5
- 🔧 JSTL and Expression Language (EL) for dynamic rendering of job data

---

## 🛠️ Tech Stack

| Layer        | Technology                                   |
|-------------|-----------------------------------------------|
| Language     | Java                                         |
| Backend      | Spring Boot (MVC)                           |
| Frontend     | JSP, JSTL, HTML5, CSS3, Bootstrap 5         |
| Styling      | Custom CSS (`style.css`, `style1.css`)      |
| Build Tool   | Maven                                        |
| Java Version | 21                                           |

---

## 🖥️ Web Interface Overview

### 🌐 Navigation

- `Home` → `/home`
- `Add Job` → `/addjob`
- `View All Jobs` → `/viewalljobs`
- `Contact` → Placeholder link

### 📝 Add Job Page (`/addjob`)

- Form fields:
  - Post ID
  - Job Title (Profile)
  - Description
  - Experience Required (Years)
  - Tech Stack (multi-select dropdown with 50+ options)

### 📋 View All Jobs (`/viewalljobs`)

- Job listings displayed in Bootstrap cards:
  - Each card shows title, description, experience, and tech stack as bullet points
  - Utilizes `c:forEach` tag and EL for dynamic content

---

## ⚙️ Maven & Dependencies

The project uses Maven for build and dependency management.

### Key Dependencies

- `spring-boot-starter-web` — Spring Boot MVC setup
- `tomcat-jasper` — JSP rendering engine
- `jakarta.servlet.jsp.jstl` — JSTL support
- `lombok` — Simplifies boilerplate (optional)
- `spring-boot-starter-test` — Testing suite

### Compiler & Build Plugins

Configured for annotation processing and Spring Boot execution:
- `maven-compiler-plugin`
- `spring-boot-maven-plugin`

---

## 🔧 Configuration

`application.properties` settings:
```properties
spring.application.name=JobApk
spring.mvc.view.prefix=/views/
spring.mvc.view.suffix=.jsp

🔮 Future Enhancements
- 🔗 Integrate JPA and a database (MySQL, H2, MongoDB)
- 🔐 Add user authentication and role-based access
- 📧 Enable email alerts for new job submissions
- 📊 Include job search and filtering capabilitie
