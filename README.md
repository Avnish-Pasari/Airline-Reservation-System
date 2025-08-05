# ✈️ Airplane Reservation System

A clean-architecture based Airline Ticket Reservation system that allows users to sign up, book flights, reschedule or refund tickets, and manage their account. Built in Java with persistent PostgreSQL storage, the system demonstrates SOLID design principles and multiple design patterns.

---

## 📖 About the Project

The **Airplane Reservation System** enables passengers to:
- **Sign Up / Sign In**
- **Book tickets** (choose flights, seats, meals, baggage)
- **Reschedule or refund tickets**
- **View booking history and account details**
- **Accumulate membership points** to unlock discounts and perks
- **Log out securely**

> ⚙️ Future plans include adding **Agent Support**, allowing agents to manage bookings for multiple customers.

---

## 🛠️ Features

- **User Management**: Sign-up, sign-in, logout, and account viewing  
- **Booking Workflow**: Flight search, seat selection, meal plan choice, baggage selection, and ticket printing  
- **Ticket Management**: Refunds, reschedules, and real-time transaction receipts  
- **Membership Tiers**: Standard, Silver, Gold, Platinum with progressive discounts  
- **Data Persistence**: PostgreSQL database integration  
- **Accessibility Considerations**: Expandable design for multiple languages and input options  

---

## 🧩 System Architecture

The project follows **Clean Architecture** and **SOLID Principles**:
- **Entities**: Core business objects (Passenger, Flight, Ticket, Seat, Meal, Baggage, Membership)  
- **Use Cases**: Application logic (BookingSystem, TransactionManager, TicketManager, PassengerSessionHandler)  
- **Interface Adapters**: Presenters, Gateways, and Factories (DataLoader, DatabaseConnector, Factories, Decorators)  
- **UI Layer**: Command Line Interface (`CmdUI`)  

**Design Patterns Implemented**:
- Template Method & Factory (Seat, Baggage, Membership creation)  
- Observer (PassengerManager updates membership points after ticket booking)  
- Iterator (Managers for Seats, Tickets, Meals, Airlines)  
- Decorator (Special features like disability discounts & baggage allowances)  
- Memento (partial implementation for rollback of seat/meal/baggage selection)  

---

## Run the program

To run the program go to `src/main/java/UI.CmdUI.java` file and run it. Follow the prompts as they are displayed to you, stick to the type of input that is asked of you to enter to avoid errors in the creation of objects according to that input.

