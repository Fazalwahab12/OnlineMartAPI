Product Service - README
Introduction:
The Product Service is responsible for managing the product catalog in the Online Imtiaz Mart API. This includes creating, updating, deleting, and retrieving product details. It interacts with the inventory service to track stock levels and ensure real-time updates.

Features:
Product CRUD Operations: Allows for the creation, retrieval, updating, and deletion of products in the catalog.
Stock Level Synchronization: Communicates with the Inventory Service to maintain up-to-date stock levels.
Event Notifications: Emits product-related events (e.g., new product added) using Kafka for other services to consume.
Efficient Data Serialization: Uses Protocol Buffers (Protobuf) for faster and efficient data serialization when communicating between services.
