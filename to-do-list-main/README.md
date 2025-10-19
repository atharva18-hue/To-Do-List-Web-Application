## To-Do List Web Application

To-Do List is a Spring Boot web application that helps users manage their daily tasks efficiently. The application allows users to create, read, update, and delete tasks. Tasks are automatically ordered based on the days remaining to complete them, ensuring better task management and prioritization.

This project demonstrates the use of Spring Boot, Spring Data JPA, Hibernate, and Maven to build a robust, full-stack web application.

Features

Add New Task: Users can create a new task by filling in a form. The form validates input and cannot be submitted until all required fields are completed.

View Tasks: All tasks are displayed in a list, ordered by the days remaining to complete each task.

Search Tasks: Users can search for tasks by title or description.

Update Task: Users can update a task using a pre-populated form.

Delete Task: Users can delete tasks they no longer need.

Task Validation: Ensures that users provide all necessary information before adding or updating tasks.

Screenshots

Task List View

<img src="https://user-images.githubusercontent.com/93772280/150697357-62b910e3-6a84-4e3e-b4f0-2b2573dac60c.PNG" width="700">

Update Task Form

<img src="https://user-images.githubusercontent.com/93772280/150697401-b4ef4206-a645-4822-8d49-4fa59189b2f3.PNG" width="700">

Add New Task Form

<img src="https://user-images.githubusercontent.com/93772280/150697411-55a03523-4888-4197-b0f2-d50bd73e6419.PNG" width="700">
Built With

Java 17

Spring Boot 2.x – Framework for building Java web applications

Spring Data JPA – Simplifies database access and ORM

Hibernate – ORM framework for mapping Java objects to database tables

Maven – Dependency management and build tool

H2/MySQL (Optional) – Database for storing tasks

Thymeleaf – Template engine for rendering dynamic HTML pages

Project Structure
To-Do-List
│
├── src/main/java
│   ├── com.example.todo
│   │   ├── controller   # Controllers for handling web requests
│   │   ├── model        # Task entity class
│   │   ├── repository   # Spring Data JPA repositories
│   │   └── service      # Service layer for business logic
│
├── src/main/resources
│   ├── templates         # Thymeleaf HTML templates
│   └── application.properties
│
└── pom.xml               # Maven dependencies

Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

Prerequisites

Java JDK 17 or above

Maven 3.x

IDE such as IntelliJ IDEA or Eclipse

Optional: MySQL database or H2 in-memory database

Installation

Clone the repository

git clone <your-repo-link>
cd To-Do-List


Build the project

mvn clean install


Run the application

mvn spring-boot:run


Access the application
Open your browser and navigate to:

http://localhost:8080/tasks

Usage

Add Task: Click “Add New Task” → Fill in the form → Submit

Update Task: Click “Edit” on a task → Modify details → Update

Delete Task: Click “Delete” on a task to remove it

Search Task: Enter a keyword in the search box → View matching results

Database Configuration

The application supports both H2 in-memory and MySQL databases. Configure your database in application.properties.

H2 Example:

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

Add user authentication and authorization

Add priority levels for tasks

Implement REST APIs for task management

Add notifications/reminders for upcoming tasks

Implement responsive UI with Bootstrap or Tailwind CSS

Author

Atharva Chavhan

GitHub: https://github.com/yourusername

LinkedIn: https://linkedin.com/in/yourprofile