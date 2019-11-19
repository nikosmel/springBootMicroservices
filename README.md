# springBootMicroservices

This is a simple Spring Boot Microservices example.
This web application does nothing more but an arithmetic service. 
An arithmetic calculator served in a microservice approach. 
The diagram below shows our two microservices, Addition Server and Subtraction Server. 
The servers need to find each other so they need to register to the discovery server called Eureka.
Once the Web Server finds the micro service, it can then send requests.
In this example, the Web Server sends RESTful requests.
When the Web Server receives the response it then serves the result to the browser.


It is easier to run the different applications by running them from the command line with different windows.
It will be eaiser to see their log output.

java -jar target/spring-boot-microservices-0.0.1-SNAPSHOT.jar eureka – executes the eureka server
java -jar target/spring-boot-microservices-0.0.1-SNAPSHOT.jar addition – executes the addition server
java -jar target/spring-boot-microservices-0.0.1-SNAPSHOT.jar subtraction – executes the subtraction server
java -jar target/spring-boot-microservices-0.0.1-SNAPSHOT.jar web – executes the web server
