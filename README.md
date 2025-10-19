# To-Do List Web Application

To-Do List is a **Spring Boot web application** that helps users manage their daily tasks efficiently. The application allows users to **create, read, update, and delete tasks**. Tasks are automatically ordered based on the days remaining to complete them, ensuring better task management and prioritization.

This project demonstrates the use of **Spring Boot, Spring Data JPA, Hibernate, and Maven** to build a robust, full-stack web application.

---

## Features

- **Add New Task:** Users can create a new task via a form. Validation ensures all required fields are filled.  
- **View Tasks:** Tasks are displayed in a list ordered by days remaining.  
- **Search Tasks:** Find tasks by title or description.  
- **Update Task:** Edit tasks using a pre-populated form.  
- **Delete Task:** Remove tasks you no longer need.  
- **Task Validation:** Ensures users provide necessary information before adding/updating tasks.

---

## Screenshots

**Task List View**  
![Task List](https://user-images.githubusercontent.com/93772280/150697357-62b910e3-6a84-4e3e-b4f0-2b2573dac60c.PNG)

**Update Task Form**  
![Update Task](https://user-images.githubusercontent.com/93772280/150697401-b4ef4206-a645-4822-8d49-4fa59189b2f3.PNG)

**Add New Task Form**  
![Add Task](https://user-images.githubusercontent.com/93772280/150697411-55a03523-4888-4197-b0f2-d50bd73e6419.PNG)

---

## Built With

- **Java 17**  
- **Spring Boot 2.x** – Java web framework  
- **Spring Data JPA** – Simplifies database access and ORM  
- **Hibernate** – ORM framework for mapping Java objects to database tables  
- **Maven** – Dependency management and build tool  
- **H2 / MySQL (Optional)** – Database for storing tasks  
- **Thymeleaf** – Template engine for rendering dynamic HTML pages

---

## Project Structure

<img width="757" height="710" alt="Screenshot 2025-10-19 082729" src="https://github.com/user-attachments/assets/91918116-4ecc-4a56-ab53-8f5c0f433ece" />

-------------------

---

## Getting Started

### Prerequisites

- Java JDK 17+  
- Maven 3.x  
- IDE (IntelliJ IDEA, Eclipse, etc.)  
- Optional: MySQL or H2 database

### Installation

1. Clone the repository:

```bash
git clone https://github.com/atharva18-hue/To-Do-List-Web-Application.git
cd To-Do-List-Web-Application

Build the project:

mvn clean install


Run the application:

mvn spring-boot:run


Open in browser:

http://localhost:8080/tasks

Usage

Add Task: Click "Add New Task" → Fill form → Submit

Update Task: Click "Edit" → Modify → Update

Delete Task: Click "Delete" → Remove task

Search Task: Enter keyword → See matching results

Database Configuration

H2 Example (in-memory database):

spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true


MySQL Example:

spring.datasource.url=jdbc:mysql://localhost:3306/todolist
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

Future Improvements

Add user authentication & authorization

Implement task priorities

Add REST APIs

Notifications/reminders for tasks

Responsive UI with Bootstrap or Tailwind CSS

Author

Atharva Chavhan

GitHub: atharva18-hue

LinkedIn: Your LinkedIn
