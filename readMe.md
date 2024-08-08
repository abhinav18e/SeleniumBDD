
# Selenium Hybrid Framework with Cucumber BDD

## Overview

This repository contains a Selenium Hybrid Framework using Cucumber BDD and Java. It integrates Extent Reports for reporting, Log4j for logging, and uses TestNG to run the tests.

## Prerequisites

- Java JDK 1.8 or higher
- Maven
- IDE (Eclipse/IntelliJ IDEA)
- ChromeDriver/GeckoDriver (based on your browser)

## Project Structure

src/
├── main/
│   ├── java/
│   │   ├── base/
│   │   ├── pages/
│   │   ├── stepDefinitions/
│   │   └── utils/
│   └── resources/
├── test/
│   ├── java/
│   │   └── runners/
│   └── resources/
│       └── features/
├── logs/
├── reports/
├── pom.xml
└── testng.xml


## Getting Started

### Clone the Repository

bash
git clone https://github.com/abhinav18e/seleniumBDD.git
cd selenium-hybrid-framework


### Install Dependencies

Run the following command to install the required dependencies:

```bash
mvn clean install
```

### Configuration

1. **Driver Configuration:** Set up the path for your WebDriver (ChromeDriver/GeckoDriver) in the `base` package.
2. **Log4j Configuration:** Configure the `log4j.properties` file located in the `resources` folder.
3. **Extent Report Configuration:** Configure the `extent-config.xml` file located in the `resources` folder.

### Running Tests

You can run the tests using TestNG:

```bash
mvn test
```

Or you can run specific feature files using the TestNG XML:

```bash
mvn test -DsuiteXmlFile=testng.xml
```

## Framework Components

### 1. Base Class

The base class initializes the WebDriver, manages browser setup, and provides utility methods for tests.

### 2. Page Classes

Page classes encapsulate web elements and actions that can be performed on them.

### 3. Step Definitions

Step definitions contain the code that implements the steps in your feature files.

### 4. Utilities

Utility classes for common operations like reading configurations, logging, and reporting.

### 5. Runners

TestNG runners to execute the feature files.

## Reporting

The framework uses Extent Reports for generating detailed test execution reports. Reports are generated in the `reports` directory.

## Logging

Log4j is used for logging. Logs are stored in the `logs` directory.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request.

## Contact

If you have any questions or feedback, feel free to reach out at abhinavnagpure4@gmail.com.
