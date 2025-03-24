# Plan and Milestones

( Created Using AI considering my busyness to better use my time for productive learning. Changes to be made as I go. )


## Milestone 1: Setup and Project Skeleton

### Duration: 
1st week

### Tasks:

Install tools: 
JDK, Node.js (for React), PostgreSQL, and an IDE (VS Code).

Create a Spring Boot project (via Spring Initializr) with dependencies: 
Spring Web, Spring Data JPA, PostgreSQL Driver, Spring Security.

Set up a React project using npx create-react-app bank-frontend.

Initialize a Git repository for version control.

### Deliverable: 
Empty Spring Boot app running on localhost:8080 and React app on localhost:3000.

Ease: Easy - basic setup, no coding logic yet.

## Milestone 2: Database and Backend Models

### Duration: 
2nd week

### Tasks:

Design database schema: Tables for Users (id, username, password, email) and Accounts (id, user_id, balance, account_number).

Configure Spring Boot to connect to PostgreSQL (update application.properties with DB credentials).

Create JPA entities (User, Account) and repositories using Spring Data JPA.

Test with a simple REST endpoint (e.g., /api/users) to fetch dummy data.

### Deliverable: 
Backend connected to PostgreSQL, returning sample user data via API.

Ease: Moderate - requires understanding JPA and database setup.


## Milestone 3: User Authentication

### Duration: 
3rd week

### Tasks:

Implement Spring Security with JWT for login/logout.

Create endpoints: /api/auth/register and /api/auth/login.

Hash passwords (e.g., using BCrypt) and store in Users table.

Test authentication with Postman.

### Deliverable: 
Secure login system where users can register and get a JWT token.

Ease: Moderate - security setup can be tricky but well-documented.


## Milestone 4: Frontend - Login and Dashboard

### Duration: 
4th week

### Tasks:

Build a React login form to call /api/auth/login.

Store JWT in local storage and redirect to a dashboard page.

Create a dashboard component to display account balance and account number (fetch from /api/accounts).

Use Axios or Fetch to connect React to Spring Boot APIs.

### Deliverable: 
Functional login page and dashboard showing account info.

Ease: Moderate - assumes basic React knowledge; API integration is straightforward.


## Milestone 5: Fund Transfer Feature

### Duration: 
5th week

### Tasks:

Add a backend endpoint /api/transfers to handle transfers (deduct from sender, add to receiver).

Update Accounts table with transaction logic (e.g., check balance, update records).

Build a React form for transfers (input: account number, amount).

Add basic validation (e.g., sufficient balance).

### Deliverable: 
Users can transfer funds between accounts via the UI.

Ease: Moderate - logic is simple but requires careful error handling.


## Milestone 6 (Optional): Deploy with Azure

### Duration: 
6th week

### Tasks:

Sign up for Azure (free tier or trial).

Deploy PostgreSQL using Azure Database for PostgreSQL.

Deploy Spring Boot backend using Azure App Service.

Host React frontend (build it and serve via Azure Static Web Apps or App Service).

Update backend config to connect to Azure PostgreSQL.

### Deliverable: 
Website live on Azure with a public URL.

Ease: 
Moderate - Azure has good docs, but cloud setup takes some learning.

## Timeline Estimate

Without Azure: ~6 weeks (depending on pace and familiarity).

With Azure: Additional ~1 week for deployment.

Total: 6-7 weeks for a functional prototype.
