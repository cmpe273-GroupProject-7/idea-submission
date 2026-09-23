# Idea submission for CMPE 273 Group project

1. High-Concurrency Ticketing / Flash Sale System

A distributed ticketing platform designed to handle thousands of users simultaneously competing for a limited number of tickets during high-demand events such as concerts, sports games, or flash sales.

The system will provide users with an event catalog, real-time ticket availability, ticket reservation, and purchase functionality. The main challenge is ensuring that limited tickets are not oversold even when thousands of requests arrive concurrently. The system will use distributed techniques such as load balancing, concurrency control, distributed locking, message queues, caching, fault tolerance, and idempotent operations to maintain consistency and availability under heavy load.

The project can be divided among four team members:

Member 1 – Event & Ticket Management: Events, ticket inventory, pricing, and availability.
Member 2 – Reservation & Concurrency: Temporary ticket holds, distributed locking, preventing double booking/overselling.
Member 3 – Payment & Order Processing: Order creation, payment simulation, asynchronous processing, and idempotency.
Member 4 – Distributed Infrastructure: API gateway/load balancing, caching, message queues, service communication, monitoring, and fault handling.

Key distributed-systems concepts:
Microservices, REST APIs, load balancing, distributed locks, caching, message queues, asynchronous processing, concurrency control, fault tolerance, idempotency, and eventual consistency.

2. Package Delivery / Logistics Platform

A distributed package delivery system that allows customers to create shipments, track packages, and receive real-time delivery updates. The system will coordinate customers, delivery drivers, warehouses, and distribution centers across multiple locations.

The main challenge is maintaining consistent package status and location information while handling a large number of concurrent shipments and updates. The system can use event-driven architecture, message queues, service discovery, load balancing, caching, and fault tolerance to process delivery events reliably.

Possible team division:

Member 1 – Customer & Shipment Service: Create shipments, addresses, package details.
Member 2 – Delivery & Driver Service: Driver assignment, delivery routes, status updates.
Member 3 – Tracking & Notification Service: Real-time tracking, notifications, event processing.
Member 4 – Distributed Infrastructure: API gateway, message queues, caching, fault handling, monitoring.

Key distributed-systems concepts:
Microservices, event-driven architecture, message queues, asynchronous processing, service discovery, load balancing, fault tolerance, eventual consistency, and distributed state management.

3. Online Auction System

A distributed online auction platform where multiple users can participate in auctions and place bids concurrently. Auctions have a defined start and end time, and the system must determine the winning bid while ensuring that concurrent bids are processed correctly and no valid bid is lost or incorrectly accepted.

The main challenge is handling high volumes of simultaneous bids while maintaining ordering, consistency, and fairness. The system can use distributed locking, event streaming, message queues, caching, and concurrency control to process bids reliably across multiple services.

Possible team division:

Member 1 – Auction Management: Create auctions, configure items, starting prices, and duration.
Member 2 – Bidding Service: Submit and validate bids, handle concurrent bidding.
Member 3 – User & Payment Service: User accounts, winner processing, and payment simulation.
Member 4 – Distributed Infrastructure: Message queues, real-time updates, caching, fault tolerance, and monitoring.

Key distributed-systems concepts:
Concurrency control, distributed locking, event-driven architecture, message queues, real-time communication, consistency, fault tolerance, idempotency, and distributed transactions.
