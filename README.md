# Event-Driven Order Management System

A Proof of Concept (PoC) demonstrating an Event-Driven Architecture using Spring Boot, Kafka, and the Saga pattern for distributed transactions.

## Architecture Overview

This project is built using the Database-per-Service pattern. It consists of the following main components:
*   **Order Service:** Handles order creation and state management (PostgreSQL).
*   **Inventory Service:** Manages product stock and handles reservations (MongoDB).
*   **API Gateway:** Routes incoming client requests to the appropriate microservices.
*   **Message Broker (Kafka):** Facilitates asynchronous communication between services.

## Tech Stack

*   **Language:** Java 21
*   **Framework:** Spring Boot 3.x, Spring Cloud
*   **Messaging:** Apache Kafka (KRaft mode)
*   **Databases:** PostgreSQL, MongoDB
*   **Infrastructure:** Docker, Docker Compose
