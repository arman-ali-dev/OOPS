### 1. What is OOPS?

OOPS stands for Object-Oriented Programming System. It is a programming paradigm based on the concept of "objects", which can contain data and code to manipulate that data.

### 2. What is Class?

A class is a blueprint for creating objects in object-oriented programming, defining properties (attributes) and behaviors (methods).

### 3. What is Objects?

An object is an instance of a class that contains its own unique data (attributes) and behaviors (methods).

### 4. What is Constructor?

A constructor is a special method that automatically executes when an object is created. It is used to initialize the object's attributes ( properties ).

### 5. What is method overloading?

Method overloading allows a class to have multiple methods with the same name but different parameters (number or type).

### 6. What is "this" keyword in java?

In Java, "this" keyword is used to refer current object.

### 7. What is Inheritance?

Inheritance is a concept where one class can use the properties and methods of another class. It helps in code reuse and better organization.

### 8. What is "super" keyword?

In Java, "super" keyword is used to refer instance of the immediate parent class.

Uses of "super" keyword in java->

1. It is used to refer variables of immediate parent class.
2. It is used to invoke a methods of immediate parent class.
3. It is used to invoke Cunstructor of immediate parent class.

### 9. What is "final" keyword?

The 'final' keyword in Java is a non-access modifier that is used to define entites that connot be changed or modified.

Final Variabled - Variables with final keyword cannot be assiged again.</br>
Final Methods - Methods with final keyword cannot be override by its subclasses.</br>
Final Class - Class with final keyword cannot be extended and inherited by other classes.

### 10. What is Encapsulation?

Encapsulation in Java means hiding data by making variables private and providing access through getter and setter methods. It helps in data security and control over how data is modified.

### 11. What is getter and setter methods?

Getter and Setter methods are used to access and modify private variables in a class.

-> Getter method returns the value of a private variable.
-> Setter method sets or updates the value of a private variable.

### 12. What is static keyword?

The static keyword in Java is used to define variables, methods, or blocks that belong to the class instead of an object.

### Key Points:

    -> Static Variable – Shared by all objects of the class.
    -> Static Method – Can be called without creating an object.
    -> Static Block – Runs once when the class is loaded.

### 13. What is Abstraction?

Abstraction means hiding the code details and showing only what is needed. It helps to focus on what an object does, not how it does it.

### 14. What is Abstract keyword?

The abstract keyword in Java is used to define abstract classes and methods that must be implemented by subclasses.

-> Abstract Class: A class that cannot be instantiated (object cannot be created).
-> Abstract Method: A method that has no body and must be implemented by child classes.

### 15. What is Interface?

In Java, an interface contains only abstract methods and static constants. It is used to achieve abstraction and multiple inheritance.

### 16. What is Inner Class?

In Java, an inner class is a class that is defined inside another class. It helps in logically grouping classes, increasing encapsulation, and making the code more readable.

### There are four types of inner classes in Java:

    -> Member Inner Class – A non-static class inside another class.
    -> Static Nested Class – A static class inside another class.
    -> Local Inner Class – A class defined inside a method.
    -> Anonymous Inner Class – A class without a name, used for one-time use.

### 17. What is Object Class?

Object class is present in java.lang package. Every class is directly and indirectly derived from Object class. if a class doesn't extended by other class then it is direct child class of the Object class.

### What is Ploymorphism?

Polymorphism in Java means the same method can behave differently based on the object that calls it. It allows flexibility and code reusability.

### Compile-Time Polymorphism (Method Overloading)

When multiple methods have the same name but different parameters, it is called compile-time polymorphism. The method is selected at compile time.

### Run-Time Polymorphism (Method Overriding)

When a subclass provides a specific implementation of a method already defined in the parent class, it is called run-time polymorphism. The method is selected at runtime.
