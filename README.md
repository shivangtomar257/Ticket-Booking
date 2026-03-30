# 🎟️ Ticket Booking System

[![Build Status](https://img.shields.io/github/workflow/status/shivangtomar257/Ticket-Booking/Java%20CI)](https://github.com/shivangtomar257/Ticket-Booking/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Issues](https://img.shields.io/github/issues/shivangtomar257/Ticket-Booking)](https://github.com/shivangtomar257/Ticket-Booking/issues)
[![Forks](https://img.shields.io/github/forks/shivangtomar257/Ticket-Booking?style=social)](https://github.com/shivangtomar257/Ticket-Booking/fork)

## 📝 Overview

Welcome to the **Ticket Booking System** — a Java (Spring Boot) web app making event ticket bookings easy and interactive! Users can search for events, book/cancel tickets, check booking history, and admins can manage everything from a user-friendly dashboard.

---

## 🚀 Quick Start

1. **Clone the repository**
    ```bash
    git clone https://github.com/shivangtomar257/Ticket-Booking.git
    cd Ticket-Booking
    ```
2. **Set Up the Database**  
   You need a running MySQL instance. Edit [`src/main/resources/application.properties`](./src/main/resources/application.properties) to set your DB user, password, URL, etc.

3. **Install dependencies & run**
    ```bash
    mvn install
    mvn spring-boot:run
    ```
4. **Open in your browser**  
   Visit: [http://localhost:8080](http://localhost:8080)

---

## 💡 Features

- 🔐 User Authentication and Authorization
- 🗓️ Browse & Search Events
- 🎟️ Book and Cancel Tickets
- ⏰ Real-Time Availability
- 💰 Integrated Payment (gateway placeholder)
- 🛠️ Admin Panel for Event Management
- 📄 REST API for automation/integration

---

## 🖥️ Technologies

[Java](https://www.java.com/) · [Spring Boot](https://spring.io/projects/spring-boot) · [Hibernate](https://hibernate.org/) · [MySQL](https://www.mysql.com/) · [Thymeleaf](https://www.thymeleaf.org/) · [Maven](https://maven.apache.org/)

---

## 📂 Project Structure

```plaintext
Ticket-Booking/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ���── com/example/ticketbooking/
│   │   └── resources/
│   └── test/
├── pom.xml
└── README.md
```
[Browse main source folder ›](./src/main/java/com/example/ticketbooking/)

---

## 🛠️ Configuration

Edit [`src/main/resources/application.properties`](./src/main/resources/application.properties) for **DB connection**, **server port**, and other environment settings.

---

## 🔥 Example User Flow

> 1. **Sign Up/Login:** Create your account or log in.
> 2. **Search Events:** Use filters for date, place, or name.
> 3. **Book Tickets:** Select available tickets and confirm payment.
> 4. **View Dashboard:** See your bookings, cancel if needed.

![User Booking Screenshot](https://github.com/shivangtomar257/Ticket-Booking/book_ticket.png)
<sup><em>_(Replace with your actual screenshots for best results.)_</em></sup>

---

## 🛡️ REST API

- All APIs return JSON; authenticate with JWT.
- Interactive API docs with [Swagger UI](http://localhost:8080/swagger-ui.html) (after starting app).

**Common Endpoints:**
- `GET /api/events` — List all events
- `POST /api/bookings` — Create new booking
- `GET /api/bookings/{id}` — Get booking details

> [Open with Postman ›](https://www.postman.com/) _(import the OpenAPI/Swagger spec if available)_

---

## 🗃️ Database Schema

| Table   | Columns                              |
|---------|--------------------------------------|
| User    | id, name, email, password            |
| Event   | id, name, date, location             |
| Booking | id, userId, eventId, status          |

---

## 🧪 Run Tests

```bash
mvn test
```

---

## 🙌 Contributing

1. **Fork** & create your branch: `git checkout -b feature/my-feature`
2. **Commit** changes: `git commit -am 'Describe feature'`
3. **Push**: `git push origin feature/my-feature`
4. **Open a Pull Request!**

[More on contributing ›](CONTRIBUTING.md)

---

## ❓ FAQ

- **App won’t start?**  
  Check your MySQL is running, config is set, and see logs for port conflicts.

- **How do I add new event types?**  
  Use the admin panel or create via API.

- **Where are configuration files?**  
  [`src/main/resources/application.properties`](./src/main/resources/application.properties)

- **Want more features?**  
  [Open an issue!](https://github.com/shivangtomar257/Ticket-Booking/issues)

---

## 📄 License

[MIT License](LICENSE)

---

> Built with ❤️ by [shivangtomar257](https://github.com/shivangtomar257)