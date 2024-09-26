Inventory Service - README
Introduction:
The Inventory Service manages stock levels and ensures that the inventory is updated in real-time when orders are placed or products are added. This service is crucial for tracking the availability of products and ensuring that stock levels are accurately reflected across the platform.

Features:
Real-Time Stock Updates: Updates stock levels when an order is placed or canceled.
Event-Driven Architecture: Listens to Kafka events related to product creation and order placement, ensuring that inventory levels are updated accordingly.
Stock Validation: Validates stock levels before confirming orders to prevent overselling.
Efficient Communication: Uses Protobuf for fast and compact communication between microservices.
