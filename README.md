# Hotel Management System

A Java-based console application for managing hotel operations, including room booking, food ordering, billing, and room deallocation. This system is designed to streamline the process of handling guest stays and enhancing the overall hotel management experience.

## Table of Contents
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Class Structure](#class-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Code Overview](#code-overview)
- [Data Persistence](#data-persistence)
- [Error Handling](#error-handling)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Room Booking**: Supports booking of luxury and deluxe rooms, both single and double.
- **Food Ordering**: Allows guests to order food items during their stay.
- **Billing System**: Automatically generates a bill that includes room charges and food costs.
- **Room Deallocation**: Facilitates checkout by deallocating rooms once the stay is complete.

## Technology Stack

- **Programming Language**: Java
- **Data Persistence**: Java Serialization (I/O)
- **User Interaction**: Command-line Interface (CLI)

## Class Structure

- **`Hotel`**: The main class that manages all core functionalities including room booking, food ordering, billing, and room deallocation.
- **`Singleroom` & `Doubleroom`**: Classes that represent single and double rooms, including attributes for customer details.
- **`Food`**: Manages food ordering functionalities and maintains details about food items and their prices.
- **`holder`**: A container class holding arrays of different room types (luxury and deluxe, single and double).

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/hotel-management-system.git
   cd hotel-management-system

2. **Compile the Java files**:
   ```bash
   javac Hotel.java
3. **Run the application**:
   ```bash
   java Hotel

## Usage

- **Room Booking**: Users can book rooms by selecting the room type (luxury or deluxe) and specifying the number of occupants.
- **Order Food**: Guests can order food from a menu of available items.
- **Generate Bill**: The system calculates the total cost, including room charges and food bills, and displays it to the user.
- **Room Deallocation**: The room is deallocated when the guest checks out, and the system becomes available for new bookings.

## Code Overview

The code is organized into several classes to achieve modularity and separation of concerns:

### `Hotel` Class

- The central class that provides a menu-driven interface for interacting with the user.
- Handles room booking, food ordering, billing, and room deallocation operations.

### `Singleroom` & `Doubleroom` Classes

- Extend basic room properties to include single and double room details.
- Manage customer information and room status.

### `Food` Class

- Manages food items, their prices, and the functionality to order food.

### `holder` Class

- Acts as a container for all rooms, maintaining separate arrays for luxury and deluxe rooms.

## Data Persistence

### Serialization

- The system uses Java serialization to save the current state of room bookings and food orders.
- Serialized data is stored in a file, allowing the system to restore the state on application restart.

## Error Handling

### Custom Exceptions

- The program includes custom exceptions like `NotAvailable` to handle specific error scenarios, such as attempting to book a room that is not available.

### User Input Validation

- The system validates user input to ensure robustness and prevent crashes due to invalid data.

## Contributing

Contributions are welcome! Please follow these steps:

1. **Fork** the repository.
2. **Create a new branch**: 
   ```bash
   git checkout -b feature-branch
3. **Commit your changes**.
   ```bash
   git commit -m "Add new feature"
4. **Push to Branch**:
   ```bash
   git push origin feature-branch
5. **Create a Pull request**;
  
   

