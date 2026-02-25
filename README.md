What is this project?

event-driven-processing-platform is a cloud-native microservices system that demonstrates asynchronous data processing using event-driven architecture.
It showcases how independent services communicate through Apache Kafka to process events reliably, scale horizontally, and remain loosely coupled.
The system is built using Spring Boot, Kafka, PostgreSQL, Docker, and Kubernetes.


Why did I build it?

To demonstrate event-driven microservices using Spring Boot and Kafka.


Architecture:

<img width="800" height="618" alt="image" src="https://github.com/user-attachments/assets/4586ab64-a4af-4e6c-9846-b50596485c56" />

<img width="3000" height="3000" alt="image" src="https://github.com/user-attachments/assets/f7a4b363-6628-44f2-a484-2e784725da7f" />

<img width="1026" height="525" alt="image" src="https://github.com/user-attachments/assets/3236feaf-997d-46ca-bbaa-a3e655f28aaf" />

<img width="1426" height="1003" alt="image" src="https://github.com/user-attachments/assets/a58ec3f0-8bad-4c63-867e-8da3d2e6f698" />



Technologies used: 
Java
Spring Boot
Kafka
PostgreSQL


Architectural Overview: Logical Flow

Client
  ↓
Controller (REST Layer)
  ↓
Service (Business Logic Layer)
  ↓
Repository (Data Access Layer)
  ↓
Database (H2 / PostgreSQL)


Each layer has a single responsibility:

Layer:Responsibility

Controller:HTTP request handling

Service:Business rules & orchestration

Repository:Persistence abstraction

Model:Domain + DB mapping


This enforces separation of concerns and keeps the system testable and maintainable.
