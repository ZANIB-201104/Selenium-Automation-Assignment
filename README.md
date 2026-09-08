# Selenium Automation

This project is a Selenium WebDriver automation framework built using Java, Maven, and TestNG.

## Technologies Used

* Java
* Selenium WebDriver
* TestNG
* Maven
* Chrome WebDriver

## Project Structure

```text
Selenium-Automation/
├── src/
│   ├── main/
│   │   └── java/
│   │       ├── org/example/
│   │       │   └── Main.java
│   │       ├── pages/
│   │       │   ├── HomePage.java
│   │       │   ├── LoginPage.java
│   │       │   └── ProductPage.java
│   │       └── utils/
│   │           └── BasePage.java
│   │
│   └── test/
│       └── java/
│           └── tests/
│               ├── LoginTest.java
│               └── ProductTest.java
│
├── pom.xml
└── README.md
```

## Prerequisites

Before running the project, make sure the following are installed:

* JDK
* Maven
* Google Chrome

Check Java installation:

```bash
java -version
```

Check Maven installation:

```bash
mvn -version
```

## How to Run

Open the terminal in the project directory and run:

```bash
mvn clean test
```

This command cleans the previous build files and executes the TestNG test cases.

## Test Cases

### Login Tests

The login tests verify:

* Successful login with valid credentials.
* Error message display when invalid credentials are provided.

### Product Tests

The product test verifies:

* Login to the application.
* Navigation to the product page.
* Product name.
* Product price.
* Product description.

## Application Under Test

The automation tests are created for the SauceDemo web application:

```text
https://www.saucedemo.com/
```

## Framework Design

The project follows the Page Object Model (POM) approach.

* `BasePage` contains common Selenium actions.
* `LoginPage` handles login-related actions.
* `HomePage` handles the home/inventory page.
* `ProductPage` handles product details.
* Test classes contain the actual test scenarios.

## Dependencies

The project uses Maven to manage dependencies, including Selenium WebDriver and TestNG.

To download dependencies, run:

```bash
mvn clean install
```

To execute tests:

```bash
mvn test
```

## Author

ZANIB ASLAM

