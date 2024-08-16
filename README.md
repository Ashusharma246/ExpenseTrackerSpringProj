Expense Tracker




Table of Contents
Introduction
Features
Technologies Used
Installation
Usage
Configuration
License
Introduction
The Expense Tracker is a Spring Boot application designed to help users manage and track their daily expenses. This project demonstrates how to create a simple yet functional expense management system using Spring Boot, Lombok, H2 Database, and Maven.

Features
Add new expenses with details such as description, amount, and date.
View a list of all expenses.
Edit or delete existing expenses.
Filter expenses by date range or category.
Persist data using H2 in-memory database.
Simple and clean UI for managing expenses.
Technologies Used
Java: The core programming language used for the application.
Spring Boot: A framework that simplifies the development of Java applications.
H2 Database: An in-memory database used for persisting data.
Lombok: A library that reduces boilerplate code by generating getters, setters, and constructors.
Maven: A build automation tool used for managing project dependencies.
Installation
Clone the repository:
sh
Copy code
git clone https://github.com/Ashusharma246/ExpenseTrackerSpringProj.git
Navigate to the project directory:
sh
Copy code
cd ExpenseTrackerSpringProj
Build the project using Maven:
sh
Copy code
mvn clean install
Run the application:
sh
Copy code
mvn spring-boot:run
Usage
Once the application is running, you can access the Expense Tracker through your web browser at http://localhost:8080.
Use the UI to add, view, edit, or delete expenses.
Configuration
Database Configuration: The application uses H2 in-memory database by default. If you want to use a different database, you can modify the application.properties file in the src/main/resources directory.

Example for using MySQL:

properties
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/expense_tracker
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
Logging Configuration: You can configure the logging level by modifying the application.properties file.

Example:

properties
Copy code
logging.level.org.springframework=INFO
logging.level.com.yourpackage=DEBUG
