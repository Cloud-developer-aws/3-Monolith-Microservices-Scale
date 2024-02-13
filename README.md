# 3-Monolith-Microservices-Scale
1. [Introduction to Microservices](#schema1)
2. [When Not to Use Microservices](#schema2)
3. [Course Outline](#schema3)
4. [AWS - Install and Configure CLI](#schema4)
5. [Monolith vs. Microservices](#schema5)


<hr>
<a name='schema1'></a>

## 1. Introduction to Microservices


**Monolitos:**

- Un monolito es una aplicación de software que se desarrolla como una única unidad o componente. Todas las funciones y características de la aplicación están empaquetadas y desplegadas juntas.
- En un monolito, todas las partes de la aplicación, como la interfaz de usuario, la lógica empresarial y la capa de datos, están interconectadas y suelen ser dependientes entre sí.
- Los monolitos son relativamente simples de desarrollar y desplegar, ya que toda la aplicación se compila y despliega como una sola entidad.
- Sin embargo, a medida que la aplicación crece en tamaño y complejidad, los monolitos pueden volverse difíciles de mantener y escalar. Además, un fallo en una parte de la aplicación puede afectar a todo el sistema.

**Microservicios:**

- Los microservicios son una arquitectura en la que una aplicación se descompone en componentes más pequeños e independientes, llamados microservicios. Cada microservicio se enfoca en una tarea específica o función de negocio.
- Los microservicios están diseñados para ser altamente cohesionados y débilmente acoplados. Esto significa que cada microservicio puede ser desarrollado, desplegado, y escalado de forma independiente sin afectar a otros componentes del sistema.
- Los microservicios se comunican entre sí a través de protocolos ligeros, como HTTP o mensajes asincrónicos. Pueden estar implementados con diferentes tecnologías y lenguajes de programación según lo que sea más adecuado para cada servicio.
- La arquitectura de microservicios facilita la escalabilidad y la flexibilidad, ya que permite a los equipos de desarrollo trabajar de forma independiente en diferentes partes de la aplicación. Sin embargo, también puede introducir complejidad en la gestión de la comunicación entre los servicios y la coordinación de las operaciones.



<hr>
<a name='schema2'></a>

## 2. When Not to Use Microservices

**Monoliths Are Not Bad!**
Microservices designs are another architectural pattern and are not intended to replace monolith applications. We should not blindly build applications as microservices without understanding the tradeoffs. Doing so could actually decrease productivity!

One way to think about this is to revisit our analogy with the Sports Superstore. Does it make sense for every aspiring small business owner to open and manage multiple stores at once?

**Considerations for Not Using Microservices**
- **System Complexity**
Rather than deploying a single application, we would be deploying multiple modules separately. There is more overhead in setting up projects.

- **Network Latency**
By introducing a network between modules, we have increased latency in application performance and will find it harder to debug our application.

- **Difficulty with Debugging**
We can no longer rely on a stack trace or tools that can help us pinpoint where a bug is. We may end up relying on logging to find causes of issues.



<hr>
<a name='schema3'></a>

## 3. Course Outline

**Microservices Design Principles and Best Practices**
- Explain different microservices architecture designs
- Divide an application into microservices

**Containers using `Docker`**
- Build and run a container image using Docker
Debug a container
- Store these images using a container registry

**Independent Releases and Deployments**
- Understand `CI/CD` benefits
- Use `Travis` to build a `CI/CD` pipeline
- Integrate `GitHub` and `CI/CD` and automate testing with CI
- Understand alternatives to `Travis` `CI` including `Jenkins`

**Service Orchestration with `Kubernetes`**
- Understand the fundamentals of `Kubernetes`

- Configure and launch an auto-scaling, self-healing `Kubernetes cluster`

- Deploy microservices using a `Kubernetes cluster`

- Understand alternative deployment strategies including `ECS` and `Fargate`

**Securing and Tuning Kubernetes Services for Production**
- Use a reverse proxy to direct requests to the appropriate backend
- Securing the microservices
- Configure scaling and self-healing for each service
- Understand the differences between internal and external traffic

**Debugging, Monitoring, and Logging** 
- Use best practices for logging with microservices
- Use logs to capture metrics for debugging
-  Implement monitoring and logging for microservices deployment
- Improve resilience and availability into cloud applications

<hr>
<a name='schema4'></a>


## 4. AWS - Install and Configure CLI

https://github.com/Cloud-developer-aws/2-Full-Stack-Apps-on-AWS


<hr>
<a name='schema5'></a>

## 5. Monolith vs. Microservices