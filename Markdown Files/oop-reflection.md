# 🧱 Object-Oriented Programming (OOP) Reflection – C#

## 🎯 Task Overview

I created a simple class hierarchy in C# involving a base class `Animal` and two derived classes: `Dog` and `Cat`. Each class overrides a virtual method to demonstrate **polymorphism**. I also implemented the **Factory design pattern** to instantiate animals based on type input.

This exercise helped reinforce key OOP concepts: **inheritance**, **polymorphism**, **encapsulation**, and **abstraction**.

---

## 🔍 Research & Learn

### ✅ The Four Pillars of OOP in C#

| Principle        | Description |
|------------------|-------------|
| **Encapsulation** | Bundles data and logic inside a class, exposing only necessary parts via public methods/properties. |
| **Abstraction**   | Hides complex implementation details, showing only relevant functionality. |
| **Inheritance**   | Allows one class to inherit properties and methods from another. |
| **Polymorphism**  | Enables methods to behave differently based on the object calling them (e.g., method overriding). |

### ✅ OOP Concepts in C# Code

- **Inheritance**: `class Dog : Animal`
- **Polymorphism**: Overriding a virtual method like `Speak()`
- **Encapsulation**: Using private fields and public properties
- **Abstraction**: Abstract base classes or interfaces define shared contracts

### ✅ Design Patterns That Use OOP Principles

- **Factory Pattern**: Uses abstraction to create objects based on input
- **Singleton Pattern**: Ensures a single shared instance
- **Strategy Pattern**: Encapsulates algorithms and selects at runtime
- **Observer Pattern**: Enables one-to-many notifications between objects

---

## 📝 Reflection

### ✅ Most Challenging Principle

**Polymorphism** was initially confusing — especially understanding how virtual and override work, and how to call base implementations if needed. Once I practiced it with different derived classes, it became clearer.

### ✅ Benefits of OOP

Applying OOP improves code **reusability**, **testability**, and **maintenance**. Shared base classes reduce duplication, and polymorphism allows flexibility when adding new types without changing existing code.

### ✅ Real-World Use Case

In a previous project, I used OOP to manage different types of users (Admin, Guest, Member) in a role-based system. Inheritance allowed shared logic, while polymorphism allowed different login behaviours — making the system scalable and easier to maintain.

---

## ✅ Summary

Understanding and applying the principles of OOP helps build well-structured, modular, and maintainable C# applications. Through class inheritance, method overriding, and design patterns like Factory, I learned how to manage complexity and write code that is easier to extend in future projects.
