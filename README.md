# IT ACADEMY BACKEND JAVA SPECIALIZATION

## SPRINT 4 TASK 1 - LEVEL 1

### Summary

This exercise serves as an initial introduction to the Spring Framework. You will begin working with the HTTP protocol, utilizing Postman, and discovering how to manage dependencies using Maven.

### Technologies

* Java (Minimum version 11)
* Spring Boot
* Maven
* HTTP

### How to run and interact with the application

1.  **Ensure Maven is installed:** Verify that Maven is installed and configured on your system.

2.  **Navigate to the project directory:** Open a terminal or command prompt and navigate to the root directory of your Spring Boot project (where the `pom.xml` file is located).

3.  **Basic Maven Commands:** Familiarize yourself with the following Maven commands:
    * **Compile the project:**
        ```bash
        mvn compile
        ```
    * **Package the project:**
        ```bash
        mvn package
        ```
    * **Clean the project:**
        ```bash
        mvn clean
        ```
    * **Run the application:**
        ```bash
        mvn spring-boot:run
        ```

4.  **Interact with the API using Postman (or a web browser):**

    * **`saluda` endpoint:**
        * Open Postman or your web browser.
        * Send a `GET` request to `http://localhost:9000/HelloWorld`. You should receive the response: `Hola, UNKNOWN. Estàs executant un projecte Maven`.
        * Send a `GET` request to `http://localhost:9000/HelloWorld?nom=YourName`. Replace `YourName` with your actual name. You should receive the response: `Hola, YourName. Estàs executant un projecte Maven`.

    * **`saluda2` endpoint:**
        * Send a `GET` request to `http://localhost:9000/HelloWorld2`. You should receive the response: `Hola, UNKNOWN. Estàs executant un projecte Maven`.
        * Send a `GET` request to `http://localhost:9000/HelloWorld2/YourName`. Replace `YourName` with your actual name. You should receive the response: `Hola, YourName. Estàs executant un projecte Maven`.

### Project Structure

The project is structured as a standard Maven project. Key files and directories include:

* `pom.xml`: Contains the project's dependencies, build configurations, and other project information.
* `src/main/java/cat/itacademy/s04/t01/n01`: Contains the main Java source code.
    * `S04T01N01Application.java`: The main entry point for the Spring Boot application.
    * `controller/HelloWorldController.java`: The REST controller handling the `/HelloWorld` and `/HelloWorld2` endpoints.
* `src/main/resources`: Contains application resources, such as the `application.properties` file.

### Notes

* This exercise provides a foundational understanding of setting up a Spring Boot project with Maven, defining REST endpoints using Spring Web, and interacting with them using HTTP.
* The use of `@RestController`, `@GetMapping`, `@RequestParam`, and `@PathVariable` annotations are key concepts in building RESTful APIs with Spring.
* Familiarizing yourself with basic Maven commands is essential for managing Spring Boot projects.
* Postman is a valuable tool for testing and interacting with your API endpoints.
