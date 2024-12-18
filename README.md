# Hello World Maven Project

This is a simple Maven project that generates a JAR file called `hello-world.jar`.
The intention of this project is to integrate GitHub Actions to automate the build and deploy process.

## Project Structure

- `src/main/java`: Contains the main Java source files.
- `src/test/java`: Contains the test Java source files.
- `pom.xml`: Project Object Model file that contains project configuration and dependencies.

## Prerequisites

- Java 21
- Maven 3.5.0 or higher

## Building the Project

To build the project and generate the JAR file, run the following command:

```sh
mvn package
```

## Running the Project
```sh
java -jar target/hello-world.jar
```

## Workflow
The workflow is defined in the `.github/workflows/maven.yml` file. It contains the following steps:
1. Checkout the code from the repository.
2. Set up Java 21.
3. Cache the Maven dependencies.
4. Extract the project version from the `pom.xml` file.
5. Install the project dependencies.
6. Build the project.