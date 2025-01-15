# Shopping Cart Spring Boot Application

## Demo Video Link : https://youtu.be/t7PKlWms5NI

## Project Overview
This project is a Shopping Cart web application built with Spring Boot. It leverages Spring Web, JPA, MySQL, and DevTools for backend development and uses HTML, CSS, and Bootstrap for the frontend. The database is managed using XAMPP's phpMyAdmin.

## Prerequisites
- **Java JDK 8 or higher**
- **IntelliJ IDEA Community Edition**
- **Maven**
- **XAMPP** (for MySQL database via phpMyAdmin)

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/shashanks20/shopping-cart-spring-boot-main.git
```

### 2. Open the Project in IntelliJ IDEA CE
- Launch IntelliJ IDEA CE.
- Click on **File > Open** and navigate to the cloned repository.

### 3. Verify Maven Installation
Ensure Maven is installed and configured properly:
```bash
mvn --version
```

### 4. Configure the Database
- Start **XAMPP** and run **Apache** and **MySQL** modules.
- Open **phpMyAdmin** by visiting [http://localhost:3306/phpmyadmin](http://localhost:3306/phpmyadmin).
- Create a new database named `ecommerce_db`.

### 5. Update Application Properties
Navigate to:
```
shopping-cart-spring-boot-main/src/main/resources/application.properties
```
Modify the following properties:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
spring.datasource.username=root
spring.datasource.password=

spring.mail.username=your-email@example.com
spring.mail.password=your-email-password
```

### 6. Run the Application
- Open `ShoppingCartApplication.java` located at:
```
shopping-cart-spring-boot-main/src/main/java/com/example/shoppingcart/ShoppingCartApplication.java
```
- Right-click the file and select **Run 'ShoppingCartApplication'**.

### 7. Access the Application
Once the application is running, access it through:
```
http://localhost:8080
```

## Project Features
- **User Registration & Authentication**: Secure user login and registration functionality.
- **Product Management**: Admin can add, update, and delete products.
- **Shopping Cart**: Users can add products to the cart, update quantities, and remove items.
- **Order Processing**: Checkout system to place orders.

## Technologies and Tools Used
### Dependencies
- **Spring Web** – To build RESTful web applications.
- **Spring Data JPA** – For ORM and database interactions.
- **MySQL Driver** – To connect Spring Boot with MySQL.
- **Spring Boot DevTools** – For live reload and development convenience.

### Tools
- **HTML, CSS, Bootstrap** – For designing the frontend UI.
- **XAMPP (phpMyAdmin)** – To manage the MySQL database.
- **SQL Database** – To store application data.
- **Spring Initializr** – To bootstrap the project setup.

