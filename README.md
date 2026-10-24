# First-Java-CRUD

A simple Java CRUD (Create, Read, Update, Delete) web application built with **Spring Boot**, **Spring Data JPA**, and **Vaadin Flow**.

---

## Features

- **Customer Management**:
  - View all customer records in an interactive Vaadin data grid (`ID`, `First Name`, `Last Name`, `Email`).
  - Real-time search/filter customers by last name.
  - Create new customer records with validation.
  - Edit customer details inline using the customer editor panel.
  - Delete customer records with one click.
- **Embedded In-Memory Database**: H2 database pre-populated with initial demo data on application startup.

---

## Prerequisites

- **Java Development Kit (JDK)**: Version 17 or 21+
- **Maven**: (Maven Wrapper `./mvnw` is included in this repository)

---

## How to Run

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd First-Java-CRUD
   ```

2. **Start the application**:
   - On Linux / macOS:
     ```bash
     ./mvnw spring-boot:run
     ```
   - On Windows:
     ```cmd
     mvnw.cmd spring-boot:run
     ```

3. **Access the Web Interface**:
   Open your browser and navigate to:
   ```
   http://localhost:8080
   ```

---

## Project Structure

```
src/main/java/com/example/demo/
├── Customer.java            # JPA entity representing customer data
├── CustomerRepository.java  # Spring Data JPA repository with custom queries
├── CustomerEditor.java      # Vaadin UI form component for adding/editing customers
├── MainView.java            # Main Vaadin UI view with data grid and filter
└── DemoApplication.java     # Spring Boot application entry point & sample data loader
```
