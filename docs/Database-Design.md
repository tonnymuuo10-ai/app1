# Database Design

## Database Management System

SQLite

## Tables

### rooms

- room_id (PK)
- room_number
- room_type
- price
- status

### customers

- customer_id (PK)
- name
- phone
- email
- address

### bookings

- booking_id (PK)
- customer_id (FK)
- room_id (FK)
- check_in_date
- check_out_date
- status

### payments

- payment_id (PK)
- booking_id (FK)
- amount
- payment_date
- payment_method

## Relationships

Customer (1) → (M) Booking

Room (1) → (M) Booking

Booking (1) → (1) Payment
