# A Ride Booking Application 🚖

A feature-rich, Uber-like application that connects riders with drivers seamlessly. Built with [Spring Boot](https://spring.io/projects/spring-boot).

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
- **Maven**: Build and dependency management.

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

---


## Prerequisites

Ensure the following are installed on your system:

- **Java 17** or later
- **Maven**
- **PostgreSQL 13** or later
- **Postman** (optional for API testing)

---


## 🔗 API Endpoints

### Authentication
| Endpoint                                   | Method | Description                        |
|-------------------------------------------|--------|------------------------------------|
| `/auth/signup`                             | POST   | Sign up a new user                |
| `/auth/login`                              | POST   | Login user and get JWT            |
| `/auth/refresh`                            | POST   | Refresh JWT token                 |

### Driver Management
| Endpoint                                   | Method | Description                        |
|-------------------------------------------|--------|------------------------------------|
| `/auth/onBoardNewDriver/{userId}`          | POST   | Onboard a new driver              |

### Rider Operations
| Endpoint                                   | Method | Description                        |
|-------------------------------------------|--------|------------------------------------|
| `/riders/requestRide`                      | POST   | Request a ride                    |
| `/riders/rateDriver`                       | POST   | Rate a driver                     |
| `/riders/cancelRide/{rideId}`              | POST   | Cancel a ride                     |
| `/riders/getMyRides`                       | GET    | Get all rides of a rider          |
| `/riders/getMyProfile`                     | GET    | Get rider profile                 |

### Driver Operations
| Endpoint                                   | Method | Description                        |
|-------------------------------------------|--------|------------------------------------|
| `/drivers/startRide/{rideRequestId}`       | POST   | Start a ride                      |
| `/drivers/rateRider`                       | POST   | Rate a rider                      |
| `/drivers/endRide/{rideId}`                | POST   | End a ride                        |
| `/drivers/cancelRide/{rideId}`             | POST   | Cancel a ride                     |
| `/drivers/acceptRide/{rideRequestId}`      | POST   | Accept a ride request             |
| `/drivers/getMyRides`                      | GET    | Get all rides of a driver         |
| `/drivers/getMyProfile`                    | GET    | Get driver profile                |

---

## API Testing

You can test these endpoints using tools like **Postman** or **cURL**. For a detailed understanding of the request body and response structure, refer to the [OpenAPI Specification](./api-docs).

---
