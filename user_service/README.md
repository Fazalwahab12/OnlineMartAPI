User Service - README
Introduction:
The User Service handles all operations related to user management in the Online Imtiaz Mart API. It manages user authentication, registration, and profile updates, ensuring secure and efficient handling of user data. This service communicates with other microservices via Kafka to notify them about user-related events, such as registration and profile updates.

Features:
User Registration: Allows users to register by creating an account with basic details such as name, email, and password.
User Authentication: Provides secure login functionality using JSON Web Tokens (JWT) for session management.
User Profile Management: Users can update their personal information (name, email, address) after registration.
Event-Driven Architecture: Produces Kafka events for actions like new user registrations, which are consumed by other services.
