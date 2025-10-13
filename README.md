# Airbnb Backend Project

## About the Project

The Airbnb Clone Project is a comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb. It involves a deep dive into full-stack development, focusing on backend systems, database design, API development, and application security. This project enables developers to understand complex architectures, workflows, and collaborative team dynamics while building a scalable web application.

## Learning Objectives

This project is tailored to enhance the expertise in modern software development practices. The developers will:

- Master collaborative team workflows using GitHub.
- Deepen their understanding of backend architecture and database design principles.
- Implement advanced security measures for API development.
- Gain proficiency in designing and managing CI/CD pipelines for efficient deployment.
- Strengthen their ability to document and plan complex software projects effectively.
- Develop an understanding of integrating technologies like Django, MySQL, and GraphQL in a unified ecosystem.
- Learn to create and manage RESTful APIs and GraphQL endpoints.
- Explore the use of Docker for containerization and deployment.
- Understand the principles of microservices architecture and its application in real-world scenarios.

## Team Roles

The project is structured to simulate a real-world development environment, with team members assigned specific roles:

- **Backend Developers**: Focus on server-side logic, database interactions, and API development.
- **Database Administrators**: Design and manage the database schema, ensuring data integrity and performance.
- **QA Engineers**: Responsible for testing, bug tracking, and ensuring the quality of the application.
- **DevOps Engineers**: Manage deployment processes, CI/CD pipelines, and infrastructure.

## Technology Stack

The project utilizes a modern technology stack to ensure scalability, performance, and maintainability:

- **Backend Framework**: Django - This high-level Python web framework encourages rapid development and clean, pragmatic design.
- **Database**: MySQL - A reliable and widely-used relational database management system.
- **API**: RESTful APIs and GraphQL - For flexible and efficient data querying.
- **Containerization**: Docker - To create, deploy, and run applications in containers.
- **Version Control**: Git and GitHub - For source code management and collaboration.
- **CI/CD**: GitHub Actions - To automate the testing and deployment processes.
- **Testing**: PyTest, Postman - For unit testing and API testing.
- **Documentation**: Markdown, Swagger - For project documentation and API documentation.

## Database Design

The core entities for the Airbnb Clone Project are:

### Users

- **Fields**: id, name, email, password_hash, date_joined
- **Description**: Represents a person using the platform. A user can own multiple properties and make multiple bookings.

### Properties

- **Fields**: id, owner_id (User), title, description, location, price_per_night
- **Description**: Represents a property listed for rent. Each property is owned by a user.

### Bookings

- **Fields**: id, user_id, property_id, start_date, end_date, status
- **Description**: Represents a reservation made by a user for a property.

### Reviews

- **Fields**: id, user_id, property_id, rating, comment, created_at
- **Description**: Represents feedback left by a user for a property after a booking.

### Payments

- **Fields**: id, booking_id, amount, payment_date, status
- **Description**: Represents payment transactions for bookings.

#### Entity Relationships

- A **User** can own multiple **Properties**.
- A **User** can make multiple **Bookings**.
- A **Booking** is linked to one **Property** and one **User**.
- A **Property** can have multiple **Reviews**.
- A **Review** is written by a **User** for a **Property**.
- A **Booking** can have one **Payment**.
