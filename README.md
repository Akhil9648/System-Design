# System Design & Design Patterns in C++

![Language](https://img.shields.io/badge/language-C++-00599C?style=flat-square&logo=c%2B%2B)
![Build](https://img.shields.io/badge/build-CMake-064F8C?style=flat-square&logo=cmake)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)

A comprehensive collection of **Object-Oriented Design Patterns** and **System Design** components implemented in modern C++. This repository documents my learning journey into low-level system architecture and scalable software design.

## 📖 Table of Contents
- [About](#-about)
- [Design Patterns Implemented](#-design-patterns-implemented)
  - [Creational](#creational)
  - [Structural](#structural)
  - [Behavioral](#behavioral)
- [System Design Components](#-system-design-components)
- [Project Structure](#-project-structure)
- [How to Build and Run](#-how-to-build-and-run)
- [Resources](#-resources)

## 🧐 About
This project aims to bridge the gap between theoretical system design concepts and practical C++ implementation. It focuses on writing clean, thread-safe, and efficient code suitable for high-performance systems.

**Key Concepts Explored:**
* Modern C++ Standards (C++14/17/20)
* Thread Safety & Concurrency (Mutexes, Atomics, Condition Variables)
* Memory Management (RAII, Smart Pointers)
* SOLID Principles

## 🧩 Design Patterns Implemented

### Creational
*Mechanisms for object creation.*
* **Singleton:** Thread-safe implementation using `std::call_once`.
* **Factory Method:** Decoupling object creation from client code.
* **Abstract Factory:** Creating families of related objects.
* **Builder:** Constructing complex objects step-by-step.

### Structural
*Class and object composition.*
* **Adapter:** Bridging incompatible interfaces.
* **Decorator:** Dynamically adding behavior to objects.
* **Facade:** Providing a simplified interface to a complex subsystem.
* **Proxy:** Controlling access to an object.

### Behavioral
*Communication between objects.*
* **Observer:** Pub-Sub mechanism for event handling.
* **Strategy:** Interchangeable algorithms (e.g., sorting, compression).
* **Command:** Encapsulating requests as objects.
* **State:** Allowing an object to alter its behavior when internal state changes.

## 🏗 System Design Components
*Low-level implementations of distributed system building blocks.*

| Component | Description | Key C++ Concepts |
| :--- | :--- | :--- |
| **LRU Cache** | Least Recently Used caching policy. | `std::list`, `std::unordered_map` |
| **Thread Pool** | Managing a pool of reusable worker threads. | `std::thread`, `std::condition_variable` |
| **Rate Limiter** | Token Bucket algorithm to control traffic. | `std::chrono`, Atomics |
| **Load Balancer** | Round Robin and Least Connection strategies. | OOP, Hashing |
| **Consistent Hashing** | Distributing data across nodes effectively. | `std::map` (BST), Hashing |

## 📂 Project Structure
```text
.
├── src
│   ├── patterns
│   │   ├── creational
│   │   ├── structural
│   │   └── behavioral
│   └── system_design
│       ├── lru_cache
│       └── thread_pool
├── include
│   └── (Header files)
├── tests
│   └── (Unit tests)
├── CMakeLists.txt
└── README.md
