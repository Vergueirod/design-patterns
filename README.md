# 📘 Personal Design patterns Guide

---

Design patterns originated from the book "Design Patterns: Elements of Reusable Object-Oriented Software" (1994), written by Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides, known as the Gang of Four (GoF). These patterns provide proven solutions to common software design problems, promoting reusability, flexibility, and maintainability.

They emerged to address challenges in object-oriented programming by capturing best practices from experienced developers. Design patterns are important because they help developers speak a common language, reduce complexity, and avoid reinventing the wheel.

---

### ALERT:

To understand design patterns WELL, a prerequisite is to understand OOP well! -> [OOP Concepts repository](https://github.com/Vergueirod/oop-concepts)

---
### Introduction: 

These **23 design patterns** are categorized into **3 groups**:
**Creational**, **Structural**, and **Behavioral** patterns.

Below is a structured list of all 23 patterns, grouped by category, each with:

* **Definition**
* **Problem they solve**
  
---

## **1. Creational Patterns**

*Focus on how objects are created and instantiated.*

1. **Singleton**

   * **Definition**: Ensures a class has only one instance and provides a global access point.
   * **Problem it solves**: You want to restrict object instantiation to a single instance (e.g., logging, configuration).

2. **Factory Method**

   * **Definition**: Defines an interface for creating an object but lets subclasses decide which class to instantiate.
   * **Problem it solves**: You want to delegate instantiation logic without specifying exact classes (e.g., a UI toolkit creating different buttons for different OS).

3. **Abstract Factory**

   * **Definition**: Provides an interface to create families of related or dependent objects without specifying their concrete classes.
   * **Problem it solves**: You need to ensure that objects from different families (e.g., Windows UI, Mac UI) work together.

4. **Builder**

   * **Definition**: Separates the construction of a complex object from its representation, allowing the same construction process to create different representations.
   * **Problem it solves**: You need to build complex objects step-by-step (e.g., building a complex document or configuration).

5. **Prototype**

   * **Definition**: Creates new objects by copying an existing object (prototype).
   * **Problem it solves**: You need to create object copies without depending on their classes (e.g., cloning a configured object).

---

## **2. Structural Patterns**

*Deal with object composition and relationships.*

6. **Adapter**

   * **Definition**: Converts the interface of a class into another interface clients expect.
   * **Problem it solves**: You want to use an existing class but its interface is incompatible.

7. **Bridge**

   * **Definition**: Decouples an abstraction from its implementation so that both can vary independently.
   * **Problem it solves**: You need to separate abstraction from implementation to avoid tight coupling (e.g., different rendering engines for shapes).

8. **Composite**

   * **Definition**: Composes objects into tree structures to represent part-whole hierarchies.
   * **Problem it solves**: You need to treat individual objects and compositions of objects uniformly (e.g., file system hierarchy).

9. **Decorator**

   * **Definition**: Adds responsibilities to an object dynamically without altering its structure.
   * **Problem it solves**: You want to extend object functionality without modifying the original class (e.g., adding scrollbars or borders to a window).

10. **Facade**

    * **Definition**: Provides a unified interface to a set of interfaces in a subsystem.
    * **Problem it solves**: You want to simplify interaction with a complex system (e.g., a library with multiple APIs).

11. **Flyweight**

    * **Definition**: Reduces the cost of creating many similar objects by sharing common parts.
    * **Problem it solves**: You need to handle a large number of objects efficiently by sharing data (e.g., characters in a text editor).

12. **Proxy**

    * **Definition**: Provides a surrogate or placeholder for another object to control access to it.
    * **Problem it solves**: You want to control access, add caching, or manage remote object interactions.

---

## **3. Behavioral Patterns**

*Focus on object interaction and responsibility distribution.*

13. **Chain of Responsibility**

    * **Definition**: Passes a request along a chain of handlers until one handles it.
    * **Problem it solves**: You want to decouple sender and receiver; multiple objects may handle the request (e.g., event handling in GUIs).

14. **Command**

    * **Definition**: Encapsulates a request as an object, allowing parameterization and queuing.
    * **Problem it solves**: You want to decouple requester from executor; also supports undo/redo operations.

15. **Interpreter**

    * **Definition**: Defines a grammar for a language and provides an interpreter to interpret sentences.
    * **Problem it solves**: You need to interpret and process language expressions (e.g., parsing expressions in a calculator).

16. **Iterator**

    * **Definition**: Provides a way to access elements of an aggregate object sequentially without exposing its internal structure.
    * **Problem it solves**: You want to traverse collections without knowing their underlying implementation.

17. **Mediator**

    * **Definition**: Defines an object that encapsulates communication between a set of objects.
    * **Problem it solves**: You want to reduce direct dependencies between interacting objects (e.g., managing UI component interactions).

18. **Memento**

    * **Definition**: Captures and restores an object’s internal state without violating encapsulation.
    * **Problem it solves**: You want to implement undo/rollback functionality.

19. **Observer**

    * **Definition**: Defines a one-to-many dependency so that when one object changes state, its dependents are notified.
    * **Problem it solves**: You want to notify multiple objects automatically of state changes (e.g., event systems, pub/sub).

20. **State**

    * **Definition**: Allows an object to change its behavior when its internal state changes.
    * **Problem it solves**: You want an object to behave differently depending on its state without large conditional logic.

21. **Strategy**

    * **Definition**: Defines a family of algorithms, encapsulates each, and makes them interchangeable.
    * **Problem it solves**: You want to switch algorithms at runtime without modifying the clients (e.g., different sorting strategies).

22. **Template Method**

    * **Definition**: Defines the skeleton of an algorithm, deferring some steps to subclasses.
    * **Problem it solves**: You want to reuse algorithm structure but allow subclasses to customize certain steps.

23. **Visitor**

    * **Definition**: Represents an operation to be performed on elements of an object structure without changing the classes of the elements.
    * **Problem it solves**: You want to add operations to object structures without modifying them (e.g., traversing object trees for reporting).

---

## **Summary Table**

| Category   | Patterns                                                                                                                        |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------- |
| Creational | Singleton, Factory Method, Abstract Factory, Builder, Prototype                                                                 |
| Structural | Adapter, Bridge, Composite, Decorator, Facade, Flyweight, Proxy                                                                 |
| Behavioral | Chain of Responsibility, Command, Interpreter, Iterator, Mediator, Memento, Observer, State, Strategy, Template Method, Visitor |

---

Each of these patterns **solves common object-oriented design problems**, promoting reusability, flexibility, and maintainability.
