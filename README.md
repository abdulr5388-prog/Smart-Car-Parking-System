# Smart Parking Management System

A Java-based desktop application that automates and streamlines parking facility management. Built with **Java Swing** for a real-time graphical interface, it handles vehicle parking, slot tracking, fee calculation, and revenue monitoring — demonstrating core **Object-Oriented Programming** principles and design patterns.

## Features

- Park **Cars** and **Bikes** using license plate input
- **Real-time slot visualization** with color-coded indicators (Green = Available, Red = Occupied)
- **Automatic fee calculation** on vehicle removal (Car: 50 PKR, Bike: 20 PKR)
- **Duplicate license plate detection**
- **Revenue tracking** displayed live on the dashboard
- 10-slot parking grid managed through a centralized Singleton class

## OOP Concepts Applied

| Concept | Implementation |
|--------|---------------|
| Interface | `Vehicle` interface implemented by `Car` and `Bike` |
| Inheritance | `Car` and `Bike` extend `Vehicle` interface |
| Polymorphism | Vehicle type handled dynamically at runtime |
| Encapsulation | Private fields with getters/setters in all classes |
| Singleton Pattern | `ParkingLot` class ensures single instance management |
| Aggregation | `ParkingLot` contains array of `ParkingSlot` objects |

## System Architecture

Vehicle (Interface)

 1) **Car**
 2)   **Bike**

ParkingSlot
    **Holds one Vehicle object**

ParkingLot (Singleton)
     **Manages 10 ParkingSlot objects + revenue tracking**

SmartParkingSystemGUI (JFrame)
     **Interacts with ParkingLot instance**


## Technologies Used

| Tool | Purpose |
|------|---------|
| Java SE 8 | Core programming language |
| Java Swing | Graphical user interface |
| IntelliJ IDEA | IDE for development & debugging |
| Git | Version control |


## How to Use

1. Enter a **license plate** in the input field
2. Click **Park Car** or **Park Bike** to assign the next available slot
3. Enter a **slot number** and click **Remove Vehicle** to free the slot and add the fee to revenue
4. Click **Show Revenue** to view total earnings

---
## UML Diagram
<img width="1020" height="668" alt="image" src="https://github.com/user-attachments/assets/8fbe1daf-7e55-4b9c-87f4-83f3d3e0d8b7" />

## Output
<img width="1023" height="604" alt="image" src="https://github.com/user-attachments/assets/8ee6b10d-0fdc-4ae4-93e0-26f693ea546a" />

