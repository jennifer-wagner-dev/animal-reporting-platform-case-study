# 🐾 Animal Reporting Platform – Case Study

A full-stack team project developed during my software development training at CODERS.BAY in Vienna.

The project addresses a practical problem: people who find an animal often do not know which organisation to contact, while missing-animal reports and found-animal reports are frequently handled separately.

The goal of the application is to provide one central platform for reporting found and missing animals and to support the process of connecting matching reports with relevant organisations.

> **Note:** This repository is a portfolio case study.  
> The original source code was developed collaboratively by a three-person team and is therefore not published here.

## 🎯 Project Context

- **Team size:** 3 developers
- **Project duration:** 5 weeks
- **Development approach:** Agile team development
- **Frontend:** Vue.js
- **Backend:** Java & Spring Boot
- **Database:** PostgreSQL
- **Communication:** REST APIs
- **Development environment:** Git, Docker

## 💡 The Problem

When someone finds an animal, the next steps are not always obvious.

Important information such as the location, time, condition of the animal and contact details needs to reach the right organisation quickly.

At the same time, owners of missing animals often publish their information through different channels.

The project aims to bring these processes together in one application.

## 🐶 Core Project Scope

The application is designed around two main workflows:

### Found Animal Reports

A user can create a structured report containing information such as:

- animal characteristics
- location and time of discovery
- injuries or immediate danger
- transport or pickup requirements
- photo
- contact information

### Missing Animal Reports

Users can report a missing animal with information such as:

- animal characteristics
- last known location
- time of disappearance
- chip or collar information
- distinguishing features
- photo
- contact information

Additional project concepts include:

- user accounts
- roles and permissions
- guest reports without a permanent account
- administration functionality
- matching found-animal and missing-animal reports
- forwarding relevant information to animal shelters or other organisations

## 🏗 Technical Architecture

The project follows a typical full-stack architecture:

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

The frontend communicates with the Spring Boot backend through REST endpoints. The backend handles application logic and persists the data in a relational PostgreSQL database.

## 👩‍💻 My Contribution

My main responsibility in the three-person team is the frontend development of the application.

I implemented most of the Vue.js frontend, including:

- user-facing views for found and missing animal reports
- organisation dashboard and case-management views
- reusable components such as navigation, cards and organisation-specific UI elements
- Vue Router configuration
- Pinia stores for organisation data, capacity and cases
- frontend data structures
- UI implementation with Vue.js and Vuetify
- integration of frontend workflows with backend APIs

The authentication store, validation logic and photo upload component were implemented by other team members.

For a more detailed breakdown of my work, see  
[My Contribution](docs/my-contribution.md).

## 🧠 What I Learned

Working on a larger team project gave me the opportunity to apply technologies that I had previously learned individually in a connected full-stack application.

In addition to technical implementation, the project involves coordinating interfaces between frontend, backend and database, discussing requirements within the team and integrating work developed by multiple people into one application.

It also helped me understand how important clear responsibilities, consistent API contracts and regular communication are when several developers work on the same system.

## 🔒 Why the Source Code Is Not Public

The application was developed collaboratively by a three-person team.

To respect the work and wishes of all contributors, the shared source code is not published in this repository.

This case study therefore focuses on:

- the problem the project addresses
- the technical architecture
- the development process
- concepts and features
- my individual contribution

without reproducing the collaborative source code.
