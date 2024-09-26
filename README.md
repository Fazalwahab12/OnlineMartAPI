Online Imtiaz Mart API - README
Project Overview:
The Online Imtiaz Mart API project aims to develop a scalable and efficient API for an e-commerce platform using an Event-Driven Microservices Architecture. The project leverages modern technologies such as FastAPI, Docker, Kafka, and PostgreSQL to ensure a high-performance, maintainable, and distributed system. The architecture is designed to handle high volumes of transactions and data while ensuring fault tolerance and resilience.

This API provides a modular and decoupled structure where services operate independently, yet communicate asynchronously through events using Kafka. The system is containerized using Docker and deployed via Azure Container Apps (ACA), with a continuous integration and deployment pipeline managed by GitHub Actions. The project follows Test-Driven Development (TDD) and Behavior-Driven Development (BDD) practices to ensure code quality and that the software meets business requirements.

Technologies Used:
FastAPI: A modern, fast (high-performance) web framework for building APIs with Python.
Docker: Containerization tool to ensure consistent deployment and operation across environments.
Kafka: A distributed event streaming platform to handle asynchronous communication between microservices.
PostgreSQL: A powerful relational database system for data persistence.
Protocol Buffers (Protobuf): Efficient serialization of structured data for communication between services.
Kong API Gateway: Manages API request routing, authentication, and rate limiting.
Azure Container Apps (ACA): Platform for cloud-native microservices and containers.
GitHub Actions: For CI/CD pipeline automation.
Pytest: Testing framework for TDD.
Behave: Framework for BDD.
Key Features:
Microservices Architecture: Each microservice in this project is self-contained and responsible for a single business functionality, such as user management, product catalog, order processing, and more. This architecture enhances modularity and allows for independent development, testing, deployment, and scaling of services.

User Service: Manages user authentication, registration, and profile management.
Product Service: Handles CRUD operations for the product catalog.
Order Service: Manages order placement, tracking, and updates.
Inventory Service: Tracks product stock levels and updates them based on orders.
Notification Service: Sends email and SMS notifications for user and order-related events.
Payment Service: Processes payments using local and international gateways (PayFast for local payments, Stripe for international).
Event-Driven Architecture:

Kafka Integration: Kafka is used as the event bus, facilitating communication between services. Each microservice can publish or subscribe to relevant events (e.g., order placed, payment processed, inventory updated).
Protobuf for Serialization: Protocol Buffers (Protobuf) is used to serialize and deserialize structured data exchanged between services, providing fast and compact message delivery.
Scalability & Resilience:

Azure Container Apps: The project is designed to scale horizontally using container-based microservices deployed to Azure Container Apps (ACA), ensuring that the system can handle high transaction volumes.
Kong API Gateway: Provides features like rate limiting, authentication, and load balancing, ensuring efficient request routing and API management.
Containerization & Orchestration:

Docker & Docker Compose: Each microservice is containerized using Docker, which ensures consistent execution across different environments. Docker Compose is used for orchestrating multi-container applications during development and testing.
DevContainers: Provides consistent development environments for all contributors, ensuring that local environments mirror production environments closely.
Database-Per-Service Pattern:

Each microservice that requires data persistence has its own independent PostgreSQL database. This ensures data isolation and improves scalability by decoupling data concerns from other services.
TDD & BDD Practices:

Test-Driven Development (TDD): All functionality is developed following TDD principles, using Pytest to write unit tests before the implementation.
Behavior-Driven Development (BDD): Using Behave, BDD ensures that business requirements are captured in natural language scenarios (Gherkin format), which are converted into automated tests. This helps align the software with business goals and ensures behavior correctness.
API Gateway (Kong):

Kong is employed as an API gateway to manage incoming client requests, apply rate limiting, handle authentication, and route requests to the appropriate microservices. It serves as a central entry point, enhancing security and reliability.
CI/CD Pipeline:

GitHub Actions: Automates the CI/CD pipeline. It runs unit tests and BDD scenarios on every push, ensuring that code is tested and validated before deployment. Deployment to Azure Container Apps is automated, ensuring continuous delivery with minimal manual intervention.
Payment Gateways:

Integration with PayFast for local transactions and Stripe for international payments ensures secure and reliable payment processing.
Logging & Monitoring (Optional Phase):

Monitoring: Tools like Prometheus and Grafana can be used for monitoring service health, performance metrics, and resource consumption.
Centralized Logging: Centralized logs from all services allow easy troubleshooting and tracking of issues across services.
Services Overview:
User Service: Handles user-related operations, including registration, login, and profile management.
Product Service: Manages products available for sale, including CRUD operations.
Order Service: Processes user orders and keeps track of order statuses.
Inventory Service: Manages product stock levels and updates them in real-time.
Notification Service: Sends email/SMS notifications for user and order updates.
Payment Service: Processes payments using PayFast and Stripe.
Getting Started:
Prerequisites:

Docker
Docker Compose
Python 3.8+
PostgreSQL
