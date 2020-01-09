# Lab 6 - Microservices and Eureka

We init service registration server Eureka, then we register
two microservices: account and web service.
![image 1](img/1 "All services deployed")
---
We can check that both microservices have been registered in Eureka
![image 2](img/2 "Microservices registered in Eureka")
---
We add another microservice account instance running on port 4444
![image 3](img/3 "2 account microservices registered in Eureka")
---
After killing microservice on port 2222, the web service still can provide
information about the accounts because account microservice running on port 4444
has replaced the one killed. For instance from the web server we try to fetch and account,
terminal running account microservice (4444) will handle the request.
![image 4](img/4 "Microservice 4444 working") 