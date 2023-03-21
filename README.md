# java-microservices-on-kubernetes
A simple microservices architecture has been designed in this educational repository using service discovery and implemented on Kubernetes. 
Eureka is used for service discovery and traffic is routed between services through the API gateway.

![Capture](https://user-images.githubusercontent.com/53411387/226596180-7c5220ce-6edd-41d4-8a20-4a327b818fbe.JPG)
After the implementation all components looks like this :
```
kubernetes@WorkerNode1:~$ kubectl get pod
NAME                                   READY   STATUS    RESTARTS   AGE
api-gateway-6885c6dc99-726sh           1/1     Running   0          2m46s
cloud-config-server-7dd6768c4c-mdqxs   1/1     Running   0          2m47s
department-service-56dbc8c8fc-v7w5p    1/1     Running   0          2m47s
eureka-744697cff9-d5k4d                1/1     Running   0          2m46s
hystrix-dashboard-bd8b6c46-f4tj2       1/1     Running   0          2m47s
user-service-7949d5b497-pt7rk          1/1     Running   0          2m48s
```

## what is Eureka ?
Service Discovery is one of the key tenets of a microservice-based architecture. Trying to hand-configure each client or some form of convention can be difficult to do and can be brittle. Eureka is the Netflix Service Discovery Server and Client. The server can be configured and deployed to be highly available, with each server replicating state about the registered services to the others.

![1](https://user-images.githubusercontent.com/53411387/226601007-b9b096ed-2963-44a5-830e-78369faabd9b.jpg)
