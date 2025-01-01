# A Ride Booking Application 🚖

A feature-rich, Uber-like application that connects riders with drivers seamlessly. Built with Spring Boot https://spring.io/projects/spring-boot.

---


## 🛠️ Tech Stack
### Backend:
- **Spring Boot**: Framework for building the backend
- **Hibernate**: ORM for database interaction
- **PostgreSQL**: Relational database
- **JWT**: Secure authentication tokens.
- **Spring Security**: Authentication and role-based authorization.
- **OpenAPI/Swagger**: API documentation.
- **Spring Boot Actuator**: Application monitoring.
- **Maven**:  Build and dependency management.



---

## 📌 Features

1. **Defining the Entities, Services, and Repositories**: Establish the core structure of the application, including models, services, and database interactions.
2. **Ride Booking**:
   - Implement `requestRide` functionality in `RiderService`.
   - Manage ride strategies with `RideStrategyManager` and implement `acceptRide` and `startRide`.
3. **Payment Support**: Add payment gateway integration for seamless transactions.
4. **Product-Ready Features**:
   - Include support for user and driver ratings.
   - Enhance real-time updates and notifications.
5. **API Documentation**:
   - Use OpenAPI and Swagger to generate comprehensive API documentation.
6. **Spring Boot Actuator**: Monitor and manage the application with built-in Actuator endpoints.
7. **Authentication and Security**:
   - Add sign-up and login using JWT.
   - Handle Spring Security exceptions effectively.
   - Implement JWT refresh tokens and access tokens.
   - Enable role-based authorization for users and admins.
8. **Email Support**: Enable email notifications for actions like ride confirmations, payment receipts, etc.
9. **Testing and Optimization**: Ensure the application is well-tested and optimized for performance and scalability.


## Prerequisites

Ensure the following are installed on your system:

- **Java 17** or later
- **Maven**
- **PostgreSQL 13** or later
- **Postman** (optional for API testing)



### 4. API Endpoints

| Endpoint                   | Method | Description                  |
|----------------------------|--------|------------------------------|
| `/api/users/signup`        | POST   | Sign up a new user           |
| `/api/users/login`         | POST   | Login user and get JWT       |
| `/api/rides/request`       | POST   | Request a ride               |
| `/api/rides/{id}/accept`   | PUT    | Accept a ride                |
| `/api/rides/{id}/start`    | PUT    | Start a ride                 |
| `/api/payments/process`    | POST   | Process a payment            |

Test these endpoints using **Postman** or similar tools.
