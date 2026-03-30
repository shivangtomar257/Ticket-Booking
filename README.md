# 🎟️ Ticket Booking System

[![Build Status](https://img.shields.io/github/actions/workflow/status/shivangtomar257/Ticket-Booking/Java%20CI/main.yml?branch=main)](https://github.com/shivangtomar257/Ticket-Booking/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Issues](https://img.shields.io/github/issues/shivangtomar257/Ticket-Booking)](https://github.com/shivangtomar257/Ticket-Booking/issues)
[![Forks](https://img.shields.io/github/forks/shivangtomar257/Ticket-Booking?style=social)](https://github.com/shivangtomar257/Ticket-Booking/fork)

---

## 📝 About the Project

Ticket Booking System is a modular Java application designed to streamline the process of searching for events, booking and cancelling tickets, and managing users in a simple, maintainable codebase.

- **User-friendly flow:** Seamlessly search, book, and manage event tickets.
- **Clean Architecture:** Clear separation between data, business logic, and utilities.
- **Ready for Expansion:** Easily add new features or integrate with a database or web front-end.

---

## 📂 Directory Structure

```
Ticket-Booking/
├── app/
│   ├── build.gradle
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── ticket/
│   │   │   │       └── booking/
│   │   │   │           ├── App.java           # Entry point
│   │   │   │           ├── entities/          # Data models
│   │   │   │           ├── localDb/           # Local data storage/DB logic
│   │   │   │           ├── service/           # Business/service classes
│   │   │   │           ├── test-ledger/       # Likely for test utilities or logging
│   │   │   │           └── util/              # Helper functions & utilities
│   │   └── test/
│   │       └── java/
│   │           └── ticket/
│   │               └── booking/
├── gradle/
├── .idea/
├── gradlew / gradlew.bat
├── README.md
└── ... (support/config files)
```

---

## 🚀 Getting Started

### Prerequisites

- Java 8 or higher
- [Gradle](https://gradle.org/install/) (or use the included wrapper `./gradlew`)

### Installation

1. **Clone the repo**
    ```bash
    git clone https://github.com/shivangtomar257/Ticket-Booking.git
    cd Ticket-Booking/app
    ```
2. **Build the project**
    ```bash
    ./gradlew build
    ```
3. **Run the application**
    ```bash
    ./gradlew run
    ```
4. **(Optional) Run tests**
    ```bash
    ./gradlew test
    ```

---

## 💡 Usage

- On running, follow CLI menus or prompts to:
  - Register or log in
  - Search for available events
  - Book and cancel tickets
  - View your booking history

> _Note: If a database or file backend is used, configure details under `localDb/` or properties files in the repo as needed._

---

## 🛠️ Technologies Used

- Java
- Gradle

_Modules and architecture support easy migration to Spring Boot, MySQL/PostgreSQL, or a web interface in the future._

---

## 📈 Extending the Project

- **Add Events:** Add new Event class objects in the `entities` package.
- **New Features:** Implement business logic in the `service` package.
- **Database Integration:** Link in the `localDb` package or add a spring-data integration.
- **API Layer:** Structure a REST API in a new `controller` package for web front-end support.

---

## 🙌 How to Contribute

We welcome bug reports, pull requests, and ideas!

1. Fork the repository
2. Create a feature branch:
    ```bash
    git checkout -b feature/amazing-feature
    ```
3. Commit your changes:
    ```bash
    git commit -m "Add: amazing feature"
    ```
4. Push to your branch and open a [Pull Request](https://github.com/shivangtomar257/Ticket-Booking/pulls)

---

## 📄 License

Distributed under the MIT License. See [LICENSE](LICENSE) for more information.

---

## 🙋 Contact

Project maintained by [shivangtomar257](https://github.com/shivangtomar257).

---

> _Happy booking! If you like this project, ⭐️ the repo and share your feedback!_
