## Project Idea for CMPE 273 Group project
# High-Concurrency Ticketing / Flash Sale System

A distributed ticketing platform for high-demand events, such as concerts or sports games, where many users compete for a limited number of tickets at the same time. The system will let users browse events, check ticket availability, reserve tickets, and complete purchases.

The platform must prevent tickets from being oversold while remaining responsive during sudden traffic spikes. It will use distributed services and coordination to handle concurrent requests reliably and keep ticket availability consistent.

## Project Challenge: Fair-Queue Ingress Processing

A flash sale can send millions of requests toward the API gateway at once. If all requests reach the application and database together, the resulting “thundering herd” can overwhelm the system before it can decide which users to serve.

We will build a distributed virtual waiting room to manage this incoming traffic. It will place users in a fair first-in, first-out (FIFO) queue, issue queue tokens across distributed nodes, and admit users at a controlled rate that matches the backend database’s transaction capacity.

The waiting room may use Redis Sorted Sets or Kafka partitions to coordinate queue positions and admission across nodes. The design should preserve queue order, avoid admitting more traffic than downstream services can handle, and continue operating reliably during a high-demand sale.

## Key Distributed-Systems Concepts

- Distributed virtual waiting rooms
- FIFO queueing and fair admission
- Redis Sorted Sets or Kafka partitions
- Rate limiting and backpressure
- Load balancing and concurrent request handling
- Distributed coordination
- Fault tolerance and idempotent operations
- Consistency between ticket availability, reservations, and purchases
