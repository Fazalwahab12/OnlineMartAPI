Payment Service - README
Introduction:
The Payment Service processes and manages payments for orders placed in the Online Imtiaz Mart API. It integrates with local and international payment gateways (PayFast for local and Stripe for international payments), ensuring secure and reliable transaction processing.

Features:
Payment Processing: Handles both local (PayFast) and international (Stripe) payment processing for user orders.
Transaction Tracking: Manages the state of transactions, tracking whether payments were successful, pending, or failed.
Event-Driven Communication: Emits and listens to Kafka events for order payments, informing other services (like the Order Service) about payment statuses.
Security: Ensures secure handling of payment information using industry-standard encryption.
