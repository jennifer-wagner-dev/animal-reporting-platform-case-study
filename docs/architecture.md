# Technical Architecture

The project follows a typical full-stack architecture using Vue.js, Spring Boot and PostgreSQL.

## Overview

```text
┌──────────────────────┐
│      Vue.js UI       │
│      Frontend        │
└──────────┬───────────┘
           │
           │ REST / JSON
           │
┌──────────▼───────────┐
│     Spring Boot      │
│       Backend        │
│                     │
│ Controller           │
│ Service              │
│ Repository           │
└──────────┬───────────┘
           │
           │ JPA / SQL
           │
┌──────────▼───────────┐
│     PostgreSQL       │
│      Database        │
└──────────────────────┘
```

## Frontend

The frontend is implemented with Vue.js and is responsible for:

- displaying application data
- handling user input
- validating form data
- communicating with the backend through REST APIs

## Backend

The backend is implemented with Java and Spring Boot.

Its responsibilities include:

- REST endpoints
- application logic
- validation
- database access
- user and role management

## Database

PostgreSQL is used as the relational database.

The database stores information such as:

- animal reports
- animal characteristics
- locations
- users
- contact information
- report status

## Communication

Frontend and backend communicate through REST endpoints using JSON.
