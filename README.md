# 🎟️ Ticket Booking System

[![Build Status](https://img.shields.io/github/actions/workflow/status/shivangtomar257/Ticket-Booking/Java%20CI/main.yml?branch=main)](https://github.com/shivangtomar257/Ticket-Booking/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Issues](https://img.shields.io/github/issues/shivangtomar257/Ticket-Booking)](https://github.com/shivangtomar257/Ticket-Booking/issues)
[![Forks](https://img.shields.io/github/forks/shivangtomar257/Ticket-Booking?style=social)](https://github.com/shivangtomar257/Ticket-Booking/fork)

---

## 📝 Overview

**Ticket Booking System** is a Java application that allows users to browse events and book tickets. It features clear modularization between booking logic, data entities, utility classes, and service layers.

---

## 📁 Project Structure

```
Ticket-Booking/
├── app/
│   ├── build.gradle
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── ticket/
│   │   │   │       └── booking/
│   │   │   │           ├── App.java
│   │   │   │           ├── entities/
│   │   │   │           ├── localDb/
│   │   │   │           ├── service/
│   │   │   │           ├── test-ledger/
│   │   │   │           └── util/
│   │   │
│   │   └── test/
│   │       └── java/
│   │           └── ticket/
│   │
│   └── build/
├── gradle/
├── .idea/
├── .gitignore
├── .gitattributes
├── gradle.properties
├── gradlew
├── gradlew.bat
├── settings.gradle
└── README.md
```

### Main Source Layout

- `app/src/main/java/ticket/booking/`
  - `App.java`: Entry point of the application.
  - `entities/`: Data model classes (e.g., User, Event, Booking).
  - `localDb/`: Data storage/DB interaction logic.
  - `service/`: Services encapsulating business logic.
  - `test-ledger/`: (Likely) test or transaction tracking helpers.
  - `util/`: Utility classes for common/reusable logic.

- `app/src/test/java/`: Test source set for unit/integration tests.

---

## 🚀 Getting Started

### Prerequisites

- Java 8+ and Gradle installed.
- (Optional) MySQL if using an external DB.

### Setup

1. **Clone the repository**
    ```bash
    git clone https://github.com/shivangtomar257/Ticket-Booking.git
    cd Ticket-Booking/app
    ```

2. **Configure the application**
    - Update DB settings if needed in resource or config files.

3. **Build and Run**
    ```bash
    ./gradlew build
    ./gradlew run
    ```

4. **Run Tests**
    ```bash
    ./gradlew test
    ```

---

## 💡 Features

- Search and browse events
- Book and cancel tickets
- User account management
- Booking management and history
- Modular code structure for maintainability

---

## 🗂️ Technologies

- Java (core language)
- Gradle (build system)

---

## 🙌 Contributing

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes
4. Push to your branch
5. Open a Pull Request!  

---

## 📄 License

[MIT License](LICENSE)

---

> Made by [shivangtomar257](https://github.com/shivangtomar257)
