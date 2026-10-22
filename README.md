# E-Commerce Domain Model & Cart System

A clean, object-oriented Java implementation modeling core e-commerce business entities, customer shopping carts, and checkout flows.

---

## 📌 Overview

This project implements fundamental domain logic for an online shopping system. It demonstrates key Object-Oriented Programming (OOP) concepts—encapsulation, abstraction, and entity aggregation—to provide a reliable baseline for an e-commerce order management backend.

---

## 🏗️ Architecture & Class Structure

The codebase is organized into domain model classes that represent the primary entities of an e-commerce platform:

| Class | Responsibility | Key Attributes / Methods |
|---|---|---|
| `Product` | Represents catalog items available for purchase | `id`, `name`, `price`, `stock`, `toString()` |
| `Cart` | Manages customer selected items in-memory | `items` (List of Products), `addProduct()`, `printItems()` |
| `User` | Encapsulates customer identity and account details | `id`, `username`, `email`, getters |
| `Main` | Entry point demonstrating product instantiation and cart aggregation | `main(String[] args)` |

---

## 🛠️ Prerequisites

- **Java Development Kit (JDK):** Version 8 or higher
- Any terminal or command line environment

---

## 🚀 Compilation & Execution

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dimrishashank/Ecommerce.git
   cd Ecommerce
   ```

2. **Compile the Java source files:**
   ```bash
   cd src
   javac *.java
   ```

3. **Run the application:**
   ```bash
   java Main
   ```

**Expected Output:**
```text
product ID: 1 name: laptop price: 100000.0 stock: 10
product ID: 1 name: laptop price: 100000.0 stock: 10
```

---

## 💡 Software Engineering Principles

- **Encapsulation:** All model properties (`id`, `name`, `price`, `stock`) are `private` with explicitly defined public accessor methods to protect internal state.
- **Composition over Inheritance:** The `Cart` utilizes composition via Java Collections (`List<Product>`) to dynamically manage item collections without rigid inheritance hierarchies.
- **Convention Adherence:** Strict Java class-to-filename naming conventions ensuring cross-platform compilation reliability across Windows, macOS, and Linux.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
