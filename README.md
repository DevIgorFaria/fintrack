# Fintrack

Fintrack is a personal finance management API built with Java and Spring Boot.

The project is being developed as a portfolio project and as a structured learning path for backend engineering. Its goal is to model a realistic financial domain while applying practices commonly used in production APIs: clean REST design, validation, persistence, database migrations, authentication, automated tests, Docker-based local development, and clear documentation.

## Overview

Fintrack is designed to help users track their personal finances by organizing accounts, categories, and financial transactions.

The application will support income and expense tracking, transaction filtering, balance calculation, monthly summaries, and private data per authenticated user.

## Main Features

Planned features include:

- Category management for income and expenses.
- Financial account management, such as wallet, checking account, savings account, and credit card.
- Income and expense transaction registration.
- Transaction filtering by date range, category, account, and transaction type.
- Account balance calculation.
- Monthly financial summaries.
- User registration and authentication.
- Data isolation so each user can only access their own financial records.

## Learning Objectives

This repository is intentionally built to practice and demonstrate backend development concepts through a practical project.

The main learning objectives are:

- Build a REST API with Spring Boot.
- Structure a Java backend project in layers.
- Model relational data with JPA and Hibernate.
- Use PostgreSQL as the application database.
- Version database changes with Flyway migrations.
- Validate request data and return meaningful API errors.
- Use DTOs to separate API contracts from persistence models.
- Write automated tests for application behavior.
- Add authentication and authorization with JWT.
- Run the project locally with Docker Compose.
- Document technical decisions clearly for a portfolio repository.

## Tech Stack

- Java 21
- Spring Boot
- Spring Web
- Spring Data JPA
- Spring Validation
- PostgreSQL
- Flyway
- Maven
- Docker Compose
- JUnit

## Project Status

Fintrack is currently in early development.

Implemented so far:

- Spring Boot application setup.
- Health check endpoint.
- PostgreSQL service configured with Docker Compose.
- Backend dependencies configured for Web, Validation, JPA, PostgreSQL, and Flyway.
- Initial category domain model with income and expense types.

Next development focus:

- Configure the application database connection.
- Add the first Flyway migration.
- Implement category CRUD endpoints.
- Add DTOs, validation, and error handling.
- Add automated tests for the first API flow.

## Roadmap

### 1. Foundation

- Configure PostgreSQL connection properties.
- Create initial database migrations.
- Validate the Maven build and test setup.
- Define base package organization.

### 2. Categories

- Create category repository.
- Create category service.
- Add request and response DTOs.
- Implement category CRUD endpoints.
- Add validation rules.
- Add tests for category creation and listing.

### 3. Accounts

- Model financial accounts.
- Implement account CRUD endpoints.
- Define account types and balance behavior.
- Add account-related tests.

### 4. Transactions

- Model financial transactions.
- Link transactions to accounts and categories.
- Implement transaction creation, update, deletion, and listing.
- Add filters by date, account, category, and type.
- Add balance and summary calculations.

### 5. Security

- Add user registration.
- Add login with JWT authentication.
- Protect private API endpoints.
- Ensure users can only access their own data.

### 6. Portfolio Readiness

- Add API documentation.
- Add example requests and responses.
- Add GitHub Actions for continuous integration.
- Add deployment instructions.
- Document architecture and technical decisions.

## Running Locally

### Requirements

- Java 21
- Docker
- Docker Compose

### Start PostgreSQL

```bash
docker compose up -d
```

### Run the Application

Linux/macOS:

```bash
./mvnw spring-boot:run
```

Windows:

```bash
.\mvnw.cmd spring-boot:run
```

### Run Tests

Linux/macOS:

```bash
./mvnw test
```

Windows:

```bash
.\mvnw.cmd test
```

## Current API


## Repository Purpose

This project is not only a finance API. It is also a record of my backend learning process.

Each feature is intended to be built incrementally, with attention to code organization, database design, tests, and documentation so the repository can show both technical progress and decision-making.
