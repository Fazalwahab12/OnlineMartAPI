Kafka - README
Introduction:
Kafka serves as the event streaming platform for the Online Imtiaz Mart API, allowing services to communicate asynchronously. Kafka facilitates real-time data flow between microservices, ensuring that messages are produced and consumed effectively.

Features:
Event Bus: Acts as the central event bus for microservices, enabling the decoupling of services through message streaming.
High Throughput: Ensures the system can handle a high volume of messages, making it scalable for large datasets and high user traffic.
Topic-Based Messaging: Organizes messages into topics, allowing services to subscribe to specific topics for events they need.
Resilience: Provides fault-tolerant and highly available messaging to ensure no loss of events during failures.
