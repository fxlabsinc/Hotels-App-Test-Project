<figure>
<img src="https://fxlabs.io/wp-content/uploads/2018/02/FX-Logo-100x100.png" alt="" />
</figure>



# Automated API Testing & Security for the Spring REST Hotels App Example

This is a test project hosting all the auto-generated and user-created tests suites for an example Spring REST application that is currently running on AWS.

### How to Run the Spring REST Hotels App Example

This application is packaged as a WAR which has Tomcat 8 embedded. No Tomcat or JBoss installation is necessary. You run it using the java -jar command.

* Clone this [GitHub Repository](https://github.com/khoubyari/spring-boot-rest-example)
* Make sure you are using JDK 1.8 and Maven 3.x
* Build the project by running ```mvn clean package```
* Once successfully built, you can run the service by one of these two methods:

```
java -jar -Dspring.profiles.active=test target/spring-boot-rest-example-0.5.0.war
OR
mvn spring-boot:run -Drun.arguments="spring.profiles.active=test"
```

### Supported REST APIs

| Method | Endpoint | Parameters | Response Messages |  
| :---         | :---           | :---          | :---         | 
| GET   | /example/v1/hotels    | page (page number), size (page size)      |  401 (Unauthorized), 403 (Forbidden), 404 (Not Found)     | 
| POST     | /example/v1/hotels      | git diff      | 401 (Unauthorized), 403 (Forbidden), 404 (Not Found)      | 
| DELETE   | /example/v1/hotels/{id}    | git status    | 401 (Unauthorized), 403 (Forbidden), 404 (Not Found)    | 
| GET    | /example/v1/hotels/{id}      | git diff      | 401 (Unauthorized), 403 (Forbidden), 404 (Not Found)      | 
| PUT   | /example/v1/hotels/{id}     | git status    | 401 (Unauthorized), 403 (Forbidden), 404 (Not Found)    |  
