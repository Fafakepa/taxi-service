# Taxi-service
![Alt Text](https://a.ltrbxd.com/resized/sm/upload/98/oj/qb/mc/8a8QjNv3Ziqc2tGjRmq34VEqMjq-1200-1200-675-675-crop-000000.jpg?v=2280b4fb73)

This is a web application to demonstrate simple CRUD operations, authentication, and registration using MySQL and servlets, without any frameworks.

## Functionality

* register as a driver;
* login as driver;
* create/update/delete a driver;
* display all drivers
* create/update/delete a car;
* display all cars;
* create/update/delete a manufacturer;
* display all manufacturers;
* add a driver to a car;
* display all cars for current login driver;

## Project Structure

The project follows a typical structure with the following components:

- **DAO:** The DAO layer receives requests from the service layer, transfers them to the database, and executes SQL queries to perform CRUD (Create, Read, Update, Delete) operations. The DAO classes encapsulate database operations and provide data persistence.
- **Service:** The service layer receives requests from the controller layer, transmits them to the DAO layer, and executes business logic. It acts as an intermediary between the presentation layer and the data access layer, performing data manipulation, validation, and processing as required.
- **Controller:** The controller layer receives requests from the user interface, transmits them to the service layer, and handles the overall flow of the application. Controllers handle HTTP requests, invoke corresponding service methods, and return appropriate responses. They are responsible for handling user input, managing session data, and coordinating the interaction between the user and the application.

## Technologies Used

The project utilizes the following technologies:

- Java 17
- Apache Tomcat 9.0.50
- MySQL 8.0.22
- Maven 3.1.1
- Java Servlet 4.0.1
- JSTL 1.2
- JSP and CSS
- JDBC

## Instructions for Launching the Project

* Clone the project from GitHub
* Use /resources/init_db.sql to create a schema and tables
* Configure /util/ConnectionUtil.java with your own URL, username, password and JDBC driver
* Configure Tomcat server
* Run and enjoy the program