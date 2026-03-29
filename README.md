# Student Management System (Spring Boot)

## Project Overview

This project is a **simple Student Management REST API** built using **Java and Spring Boot**.
The application allows users to perform basic **CRUD operations** on student records such as adding a student, viewing students, and deleting students.

The main purpose of this project is to demonstrate the **basic concepts of Spring Boot**, including REST APIs, controllers, repositories, and entity mapping.

This project is designed as a **beginner-level backend project** to understand how a Spring Boot application works.

---

## Features

The application supports the following operations:

* Add a new student
* View all students
* Get a student by ID
* Delete a student

These operations are performed through **REST API endpoints**.

---

## Technologies Used

The following technologies are used in this project:

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* H2 Database (in-memory database)

---

## Project Structure

This project contains the following main files:

* **StudentManagementApplication.java**
  This is the main class that starts the Spring Boot application.

* **Student.java**
  This class represents the Student entity and defines the structure of student data.

* **StudentRepository.java**
  This interface handles database operations using Spring Data JPA.

* **StudentController.java**
  This class defines REST API endpoints to manage student records.

---

## API Endpoints

### Add Student

POST `/students`

Example request body:

```json
{
"name": "Rahul",
"course": "Computer Science",
"age": 21
}
```

---

### Get All Students

GET `/students`

Example response:

```json
[
 {
  "id": 1,
  "name": "Rahul",
  "course": "Computer Science",
  "age": 21
 }
]
```

---

### Get Student by ID

GET `/students/{id}`

Example:

```
GET /students/1
```

---

### Delete Student

DELETE `/students/{id}`

Example:

```
DELETE /students/1
```

---

## How the Application Works

1. The user sends a request to the API.
2. The **Controller** receives the request.
3. The controller calls the **Repository**.
4. The repository interacts with the database.
5. The response is returned to the user.

---

## Learning Purpose

This project was created to practice:

* Spring Boot basics
* REST API development
* CRUD operations
* Backend application structure

It is a simple example project for learning **backend development using Spring Boot**.

---

## Author
Nitish Kumar
