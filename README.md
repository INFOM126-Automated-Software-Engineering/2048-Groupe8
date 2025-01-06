# 2048
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=INFOM126-Automated-Software-Engineering_2048-Groupe8&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=INFOM126-Automated-Software-Engineering_2048-Groupe8)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=INFOM126-Automated-Software-Engineering_2048-Groupe8&metric=coverage)](https://sonarcloud.io/summary/new_code?id=INFOM126-Automated-Software-Engineering_2048-Groupe8)

Welcome to the 2048 game, implemented in Java!

# Requirements

Ensure the following tools are installed on your system:

    Java JDK (Version 11 or later)
    Maven (Version 3.6 or later)

# Getting Started
1. Clone the Repository

       git clone https://github.com/INFOM126-Automated-Software-Engineering/2048-Groupe8.git
       cd 2048-Groupe8

2. Build the Project with Maven

Use Maven to compile the code and package the application:

    mvn clean install

3. Run Tests

Run unit tests to ensure the application works as expected:

     mvn test

4. Generate Coverage Report

To generate the code coverage report using Jacoco:

    mvn jacoco:report

The report will be available in:

target/site/jacoco/index.html

5. Deploy the Application

You can deploy the application using Maven's deploy plugin. Make sure to configure the distributionManagement section in your pom.xml file or provide a repository URL using the command-line option:

        mvn deploy -DaltDeploymentRepository=<id>::<layout>::<url>

Example:

mvn deploy -DaltDeploymentRepository=my-repo::default::http://your-repo-url

# Usage
Run the Application

After building the project, you can run the game:

      java -jar target/2048-Groupe8-<version>.jar

Replace <version> with the appropriate version number of the packaged JAR file.
#Contribution Guidelines

We welcome contributions! Please refer to CONTRIBUTOR.md for details on branch management, commit message conventions, and release policies.

# CI/CD Pipeline

This project uses GitHub Actions for CI/CD:

    Automatically builds and tests code on every pull request.
    Runs static code analysis with SonarQube.
    Generates a coverage badge based on Jacoco reports.

It use multiple Github actions! You can view the CI/CD workflow files in the .github/workflows/ directory.

# License

This project is licensed under the MIT License. See the LICENSE file for more details.
# Contact

For any questions or issues, please open an issue or contact the development team.
