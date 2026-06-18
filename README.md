# Project LMG: State-Driven Console Inventory Management System (IMS)

An enterprise-inspired console application designed to execute administrative CRUD operations and persistent data management utilizing a strict Object-Oriented State Design Pattern.

---

## Engineering & Architectural Achievements

* **State Design Pattern Implementation:** Eliminated monolithic conditional branching loops by architecting a formalized Behavioral State Pattern. Each system view (e.g., `MainMenu`, `EditItemMenu`, `Logout`) exists as a discrete class inheriting from a base `State` wrapper, mapping user interactions directly to dynamic runtime state mutations (`system.changeState()`).
* **Complete CRUD Engine:** Built robust create, read, update, and delete subsystems allowing authenticated administrators to safely manipulate relational database abstractions for categories and sequential inventory items.
* **Decoupled Data Pipeline:** Implemented an on-demand data ingestion pipeline (`readData()`) that decouples file/database IO transactions from the visual execution layer, utilizing lazy-loading logic to statefully verify cache stability before operations.
* **Rigorous Input Validation Framework:** Integrated a centralized verification wrapper (`user_input.getIntRange`) to intercept, sanitize, and validate user entries against specific type boundaries, ensuring complete protection against boundary exceptions and execution crashes.

---

## Development Stack & Design Specs
* **Language:** Python 3
* **Design Pattern:** State Pattern (Gang of Four Behavioral Design)
* **Core Functions:** Role Authentication, Persistent Cache Handling, Context-Aware Screen Routing
* **Methodology:** Component Decoupling & Modular Architecture

---

## The Portfolio Connection (Architectural Foundation)
This project highlights a mature understanding of high-level software engineering design patterns and decoupled system architecture. The structural expertise developed here regarding state validation, runtime flow alteration, and boundary sanitization bridges directly into cybersecurity—specifically when analyzing how finite state machines handle network handshake transitions, session management, and parsing engine validation rules.
