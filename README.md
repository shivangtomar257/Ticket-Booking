# Ticket Booking System

## Overview
This is a comprehensive Java-based ticket booking application that facilitates the booking of tickets for various events and services. The application allows users to search for events, book tickets, view bookings, and manage payments.

## Features
- User authentication and authorization
- Event search functionality
- Ticket booking and cancellation
- Real-time availability updates
- Payment gateway integration
- Admin panel for event management

## Technologies
- Java
- Spring Boot
- Hibernate
- MySQL
- Thymeleaf
- Maven

## Project Structure
```
Ticket-Booking/
|-- src/
|   |-- main/
|   |   |-- java/
|   |   |   |-- com/
|   |   |   |-- example/
|   |   |   |   |-- ticketbooking/
|   |   |-- resources/
|   |-- test/
|-- pom.xml
|-- README.md
```

## Prerequisites
- Java 11 or above
- Maven 3.6 or above
- MySQL

## Installation Guide
1. Clone the repository:
   ```bash
   git clone https://github.com/shivangtomar257/Ticket-Booking.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Ticket-Booking
   ```
3. Install dependencies:
   ```bash
   mvn install
   ```
4. Set up your database and update the `application.properties` file with your database credentials.
5. Run the application:
   ```bash
   mvn spring-boot:run
   ```

## Usage Examples
- To book a ticket, navigate to the booking section in the application and follow the prompts.
- Users can view their bookings in the user dashboard.

## API Endpoints
- `GET /api/events` - Retrieve a list of all events.
- `POST /api/bookings` - Create a new booking.
- `GET /api/bookings/{id}` - Retrieve booking details.

## Database Schema
- **User**: `id`, `name`, `email`, `password`
- **Event**: `id`, `name`, `date`, `location`
- **Booking**: `id`, `userId`, `eventId`, `status`

## Configuration
Configuration details can be found in the `application.properties` file, including database connection and server port.

## Testing
Run tests using:
```bash
mvn test
```

## Contributing Guidelines
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## Troubleshooting
- If the application fails to start, check the logs for errors related to port conflicts or database connection.
- Ensure all prerequisites are met.

## License
This project is licensed under the MIT License.