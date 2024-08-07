# CarRentify

CarRentify is a car rental system based on a microservices architecture, built with .NET.
The system allows users to register, browse available vehicles, make reservations, and manage their bookings.

## Microservices

- **Customer Service:**
  - Features
    - User registration and login
    - Profile management
  - Technologies
    - .NET 8
    - Postgres with Entity Framework Core
    - CQRS with MediatR
    - Vertical slices

- **Vehicle Service:**
  - Features
    - Add and manage vehicles
    - Categorize vehicles
  - Technologies
    - .NET 8
    - Postgres with Marten
    - Vertical slices

- **Booking Service:**
  - Features
    - Create, modify, and cancel bookings
    - Manage booking history
    - Payment processing
  - Technologies
    - .NET 8
    - Postgres with Marten
    - Vertical slices
    - Event Sourcing

- **Customer API Gateway:**
  - Features
    - Entry point for external clients
    - Routing to appropriate microservices
    - Manage routing, authorization, and rate limiting

- **Backoffice API Gateway:**
  - Features
    - Entry point for internal users
    - Routing to appropriate microservices
    - Manage routing, authorization, and rate limiting

## Infrastructure
- PostgreSQL
- Kafka
- RabbitMQ

## Getting Started

### Prerequisites

- Docker

### Running Locally

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/CarRentify.git
    cd CarRentify
    ```

2. Set up the necessary infrastructure using Docker Compose:
    ```sh
    docker-compose up -d
    ```
