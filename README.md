# spring-core-notes
My learning notes on Spring and Spring Boot (IOC, DI, Beans, Scopes, Lifecycle).

(Beginner to Pro Notes)

Overview

This repository contains my deep understanding of Spring Framework and Spring Boot, focusing on the core concepts that every backend engineer must master before building real-world applications.

These notes simplify the internal working of Spring — IOC, DI, Beans, Autowiring, Scopes, Lifecycle — in a clean, developer-friendly way.

 1. Inversion of Control (IOC)

IOC is a design principle where Spring manages object creation, not the developer.
Instead of using:

UserService service = new UserService();


Spring creates and controls these objects automatically.
This reduces tight coupling and makes applications scalable.

 2. Dependency Injection (DI)

DI allows Spring to inject required dependencies into classes.

Types of DI:

Constructor Injection (Best practice)

Setter Injection

Field Injection (@Autowired)

Spring decides how to inject beans based on annotations and matching types/names.

 3. Spring Beans

Beans are objects that Spring manages.
Classes annotated with:

@Component

@Service

@Repository

@RestController

…are automatically detected and registered as beans.

 4. Bean Lifecycle

Spring manages the full lifecycle of a bean:

Instantiation

Dependency Injection

Post-initialization (@PostConstruct)

Ready for use

Destruction (@PreDestroy)

 5. Bean Scopes

Different scopes define how many instances of a bean exist:

Singleton (default – one instance for entire app)

Prototype (new instance every time)

Request (per HTTP request)

Session (per user session)

 6. Autowiring Process

Spring chooses beans in this order:

By type

By name

Using @Qualifier

Using @Primary

Otherwise → throws NoUniqueBeanDefinitionException

7. Spring Boot

Spring Boot simplifies Spring with:

Auto-configuration

Embedded server

Easy project setup (Spring Initializr)

No XML configuration

Production-ready features

You write less code and build faster.

 Conclusion

These concepts form the foundation of building REST APIs, Microservices, and enterprise Java applications.

Next steps:

Build REST controllers

Add Service + Repository layers

Use Spring Data JPA

Implement JWT Authentication

⭐ About This Repository

This repo documents my learning journey as I prepare to become a professional backend developer focusing on Spring Boot and enterprise Java development.
