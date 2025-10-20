# Airbnb Clone Project

## Overview
This project is a full-stack Airbnb clone designed to simulate a real-world booking platform. It focuses on backend development, database design, API development, and security, providing hands-on experience in building scalable web applications.

---

## Team Roles

- **Backend Developer:** Builds and maintains server-side logic, APIs, and database interactions.
- **Database Administrator:** Designs and manages the database structure, ensuring data integrity and performance.
- **Frontend Developer:** Implements the user interface and integrates it with backend APIs.
- **DevOps/CI-CD Engineer:** Sets up automated pipelines for testing, deployment, and monitoring.
- **QA Engineer:** Tests features to ensure quality and security compliance.

---

## Technology Stack

- **Django:** Web framework used for building RESTful APIs and server-side logic.
- **MySQL:** Relational database system to store and manage application data.
- **GraphQL:** API query language to efficiently fetch and manipulate data.
- **Docker:** Containerization tool to streamline development and deployment.
- **GitHub Actions:** CI/CD tool for automating testing and deployment pipelines.

---

## Database Design

### Entities:

- **Users**
  - Fields: id, name, email, password, role
  - Relationship: One user can have multiple properties and bookings

- **Properties**
  - Fields: id, title, description, location, owner_id
  - Relationship: Belongs to a user, has many bookings and reviews

- **Bookings**
  - Fields: id, property_id, user_id, start_date, end_date
  - Relationship: Linked to a property and a user

- **Reviews**
  - Fields: id, property_id, user_id, rating, comment
  - Relationship: Linked to a property and a user

- **Payments**
  - Fields: id, booking_id, amount, payment_method, status
  - Relationship: Linked to a booking

---

## Feature Breakdown

- **User Management:** Registration, login, profile management
- **Property Management:** Add, update, view, and delete properties
- **Booking System:** Reserve properties, manage bookings
- **Reviews:** Submit ratings and feedback for properties
- **Payments:** Secure payment processing for bookings

---

## API Security

- **Authentication:** Ensures only registered users can access certain features
- **Authorization:** Restricts user actions based on roles and permissions
- **Rate Limiting:** Prevents abuse by limiting API requests per user
- **Data Protection:** Secures sensitive data such as passwords and payment information

---

## CI/CD Pipeline

- **Continuous Integration:** Automated testing of code changes using GitHub Actions
- **Continuous Deployment:** Automated deployment to staging or production using Docker containers
- **Benefits:** Reduces errors, speeds up deployment, ensures consistent code quality

---

## Manual Review

All project files and documentation have been completed and pushed to the GitHub repository. The project is ready for manual QA review.
