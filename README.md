# Car Rental System

## Overview
The Car Rental System is a Java-based application that allows customers to rent and return cars. The system maintains a list of available cars, manages customer information, and handles rental transactions.

## Features
- Add new cars to the rental inventory.
- Add new customers.
- Rent a car to a customer for a specified number of days.
- Return a rented car.
- Calculate the total rental price based on the number of days.

## Classes and Responsibilities
### 1. Car
Represents a car in the rental system.
- **Attributes**:
  - `carId`: Unique identifier for the car.
  - `brand`: Car brand.
  - `model`: Car model.
  - `basePricePerDay`: Daily rental price.
  - `isAvailable`: Availability status.
- **Methods**:
  - `calculatePrice(int rentalDays)`: Calculates the total rental price.
  - `rent()`: Marks the car as rented.
  - `returnCar()`: Marks the car as available.

### 2. Customer
Represents a customer in the rental system.
- **Attributes**:
  - `customerId`: Unique identifier for the customer.
  - `name`: Customer name.

### 3. Rental
Represents a rental transaction.
- **Attributes**:
  - `car`: The rented car.
  - `customer`: The customer who rented the car.
  - `days`: Number of days the car is rented.

### 4. CarRentalSystem
Manages the overall car rental system.
- **Attributes**:
  - `cars`: List of available cars.
  - `customers`: List of customers.
  - `rentals`: List of current rentals.
- **Methods**:
  - `addCar(Car car)`: Adds a new car to the system.
  - `addCustomer(Customer customer)`: Adds a new customer to the system.
  - `rentCar(Car car, Customer customer, int days)`: Rents a car to a customer.
  - `returnCar(Car car)`: Returns a rented car.
  - `menu()`: Displays the main menu and handles user interactions.

## Getting Started
### Prerequisites
- Java Development Kit (JDK) installed.

### Running the Application
1. Clone the repository:
   ```sh
   git clone https://github.com/rishabh137/car-rental.git