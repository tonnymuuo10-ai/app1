# Hotel Management System

## Project Overview

The Hotel Management System is a Java-based application designed to automate hotel operations such as room management, customer registration, booking management, check-in/check-out processing, payment handling, and report generation.

The system aims to improve efficiency, reduce manual errors, and provide accurate record keeping for hotel operations.

---

## Objectives

- Manage hotel rooms
- Register and manage customers
- Handle room bookings
- Process customer check-ins
- Process customer check-outs
- Generate bills and payments
- Generate management reports
- Store data permanently using SQLite

---

## Features

### Room Management
- Add rooms
- Update room information
- Delete rooms
- Search rooms
- View room availability

### Customer Management
- Register customers
- Update customer details
- Search customers
- View customer history

### Booking Management
- Create bookings
- Modify bookings
- Cancel bookings
- Check room availability

### Check-In and Check-Out
- Verify bookings
- Assign rooms
- Generate bills
- Release rooms after checkout

### Reporting
- Occupancy reports
- Revenue reports
- Customer history reports
- Room utilization reports

---

## Technologies Used

| Technology | Purpose |
|------------|---------|
| Java | Main programming language |
| Gradle | Build automation tool |
| SQLite | Database |
| JDBC | Database connectivity |
| Git | Version control |
| GitHub | Source code hosting |
| JavaFX | Graphical User Interface |
| JUnit 5 | Unit testing |
| Draw.io / Lucidchart | UML diagrams |

---

## System Architecture

The project follows a layered architecture:

```
Presentation Layer (JavaFX)
        ↓
Business Layer (Services)
        ↓
Data Access Layer (DAO)
        ↓
SQLite Database
```

---

## Project Structure

```text
Hotel-Management-System
│
├── docs
├── database
├── screenshots
│
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com.hotel
│   │   │       ├── app
│   │   │       ├── model
│   │   │       ├── dao
│   │   │       ├── service
│   │   │       ├── database
│   │   │       ├── exception
│   │   │       ├── util
│   │   │       └── report
│   │   │
│   │   └── resources
│   │
│   └── test
│       └── java
│
├── build.gradle
├── settings.gradle
├── README.md
└── LICENSE
```

---

## Database Tables

### rooms

| Field | Type |
|---------|---------|
| room_id | INTEGER |
| room_number | TEXT |
| room_type | TEXT |
| price | REAL |
| status | TEXT |

### customers

| Field | Type |
|---------|---------|
| customer_id | INTEGER |
| name | TEXT |
| phone | TEXT |
| email | TEXT |
| address | TEXT |

### bookings

| Field | Type |
|---------|---------|
| booking_id | INTEGER |
| customer_id | INTEGER |
| room_id | INTEGER |
| check_in_date | TEXT |
| check_out_date | TEXT |
| status | TEXT |

### payments

| Field | Type |
|---------|---------|
| payment_id | INTEGER |
| booking_id | INTEGER |
| amount | REAL |
| payment_date | TEXT |
| payment_method | TEXT |

---

## UML Diagrams

The project includes:

- Use Case Diagram
- ER Diagram
- Class Diagram

These diagrams can be found in the `/docs` folder.

---

## Installation

### Clone Repository

```bash
git clone https://github.com/your-username/Hotel-Management-System.git
```

### Navigate to Project

```bash
cd Hotel-Management-System
```

### Build Project

```bash
gradle build
```

### Run Application

```bash
gradle run
```

---

## Testing

Run tests using:

```bash
gradle test
```

---

## Future Improvements

- Authentication system
- Admin dashboard
- Receptionist dashboard
- Email notifications
- Booking reminders
- Revenue analytics
- Charts and reports
- Online reservations

---

## Author

Bachelor of Science in Applied Computer Science Project

Hotel Management System
