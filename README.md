# coremicroservices
Microservices


Microservices->
2 or more Spring Boot module communicate with each other

1. DepartmentService- 9191
2. EmployeeService- 9192
3. ServiceRegistry- 8761[Eureka Server]
4. APIGateway- 2023
5. HystrixDashboard- 9193[Monitor our system health]

Zipkin & Sleuth- Trace distributed log

For Eureka Server-
server.port=8761
spring.application.name=ServiceRegistry
eureka.client.register-with-eureka= false
eureka.client.fetch-registry= false

Hystrix Status->
http://localhost:2023/actuator/hystrix.stream

http://localhost:9195/hystrix

API Gateway
spring.main.allow-circular-references: true
