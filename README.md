# Movie Ticket Booking System

A database schema for cinema ticket booking management.

![cinema_schem](https://github.com/user-attachments/assets/3331860b-8001-411b-99d3-5b7eb7f0093b)

## Tables

### 🎬 Movies
- Stores movie information
- Contains title, description, genre, rating

### 👥 Users
- Manages user accounts
- Includes name, email, password, contact info

### 🏢 Cinema
- Holds cinema venue details
- Tracks location and basic info

### ⏰ Showtimes
- Links movies with screening times
- Manages pricing and screen allocation

### 💺 Seats
- Controls seat inventory
- Defines seat types and numbers

### 📝 Bookings
- Records ticket reservations
- Tracks booking status and total price

### 📋 Booking Details
- Maps seats to bookings
- Stores individual seat prices

### 💳 Payments
- Processes transaction records
- Monitors payment status

## Relationships

- Movies → Showtimes (1:N)
- Showtimes → Bookings (1:N)
- Bookings → Seats (N:M)
- Users → Bookings (1:N)
- Bookings → Payments (1:1)

## Features

- Movie management
- User authentication
- Seat reservation
- Payment processing
- Booking history

## Tech Stack

- Database: PostgreSQL
- Schema Type: Relational
- Key Types: Integer, Varchar, Timestamp, Numeric
