Order Service - README
Introduction:
The Order Service handles the creation, updating, and tracking of orders placed by users. It processes user orders, ensures payment validation, and triggers inventory updates. This service communicates with the Inventory and Payment services via Kafka to manage stock and payment processing efficiently.

Features:
Order Creation: Allows users to place orders, capturing details like products, quantities, and delivery information.
Order Tracking: Provides real-time updates on the status of orders, such as order processing, shipping, and delivery.
Kafka Integration: Emits and consumes events related to order placement and updates, ensuring communication with other microservices like Inventory and Notification services.
Payment Handling: Communicates with the Payment Service to verify and process payments.
