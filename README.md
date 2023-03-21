# java-microservices-on-kubernetes
A simple microservices architecture has been designed in this educational repository using service discovery and implemented on Kubernetes. 
Eureka is used for service discovery and traffic is routed between services through the API gateway.

![Capture](https://user-images.githubusercontent.com/53411387/226596180-7c5220ce-6edd-41d4-8a20-4a327b818fbe.JPG)
## what is Eureka ?
Service Discovery is one of the key tenets of a microservice-based architecture. Trying to hand-configure each client or some form of convention can be difficult to do and can be brittle. Eureka is the Netflix Service Discovery Server and Client. The server can be configured and deployed to be highly available, with each server replicating state about the registered services to the others.

![1](https://user-images.githubusercontent.com/53411387/226601007-b9b096ed-2963-44a5-830e-78369faabd9b.jpg)
