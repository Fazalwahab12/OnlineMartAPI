API Gateway (Kong) - README
Introduction:
The Kong API Gateway manages the routing, authentication, and rate limiting of API requests in the Online Imtiaz Mart API. It serves as the entry point for all external client requests and distributes them to the appropriate microservices.

Features:
Request Routing: Manages and routes API requests to the appropriate microservice based on the request URL and method.
Authentication and Authorization: Ensures that API requests are authenticated, and only authorized users can access specific resources.
Rate Limiting: Protects the services by limiting the number of requests a client can make within a certain time period.
Load Balancing: Distributes requests across multiple instances of microservices to ensure high availability and scalability.
