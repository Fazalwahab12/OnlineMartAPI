Notification Service - README
Introduction:
The Notification Service handles user notifications related to their activities on the platform, such as order confirmations, shipping updates, and payment statuses. Notifications are sent via email or SMS, ensuring users stay informed throughout their shopping experience.

Features:
Order Status Notifications: Sends real-time notifications to users when the status of their order changes.
User Registration Notifications: Sends a welcome email or SMS upon successful user registration.
Event-Driven Notifications: Consumes Kafka events emitted by other services (e.g., Order Service) and triggers corresponding notifications.
Email/SMS Support: Provides both email and SMS notifications depending on user preferences.
