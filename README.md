# Redis Multi-Project Spring Boot Application

This is a multi-project Gradle-based Spring Boot application that includes shared dependency management and multiple
services (`service-a`, `service-b`, etc.). The project is designed to demonstrate modular development with Spring Boot
and Gradle.

## Project Structure

redis/
├── build.gradle               # Root Gradle build file with shared dependencies
├── settings.gradle            # Gradle settings file for multi-project setup
├── service-a/                 # Subproject: Service A
│   ├── build.gradle           # Service A-specific Gradle build file
│   └── src/                   # Source code for Service A
├── service-b/                 # Subproject: Service B
│   ├── build.gradle           # Service B-specific Gradle build file
│   └── src/                   # Source code for Service B
└── service-c/                 # Subproject: Service C
├── build.gradle           # Service C-specific Gradle build file
└── src/                   # Source code for Service C

## Features

- **Shared Dependency Management**: Centralized dependency versions in the root `build.gradle`.
- **Spring Boot Integration**: Each service is a Spring Boot application.
- **Modular Design**: Each service can have its own dependencies and configurations.
- **Database Support**: PostgreSQL integration for data persistence.
- **Redis Support**: Redis integration for caching.

## Prerequisites

- Java 17 or higher
- Gradle 7.6 or higher
- PostgreSQL database
- Redis server

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/redis-multi-project.git
cd redis-multi-project