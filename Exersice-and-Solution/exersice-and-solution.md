### Basic Level Questions

### 1. Create a Car class with properties: brand, model, and year.

    I. Write a constructor to initialize these values.
    II. Create an object of Car and print its properties in the console.

Ans:

```java
public class OOPS {

    public static void main(String[] args) {
        Car c1 = new Car("Mahindra", "s11", 2024);

        System.out.println("Car Brand: " + c1.brand + "\nModel: " + c1.model + "\nManufacture Year: " + c1.year);
    }

}

class Car {
    String brand;
    String model;
    int year;

    Car(String brand, String model, int year) {
        this.brand = brand;
        this.model = model;
        this.year = year;
    }
}
```

### 2. Encapsulation:

    I. Create a BankAccount class where balance is private.
    II. Write a deposit(amount) method to increase the balance.
    III. Write a withdraw(amount) method to check and then decrease the balance.

Ans-

```java
public class OOPS {

    public static void main(String[] args) {
        BankAccount b1 = new BankAccount();
        b1.deposit(1000);
        b1.withdraw(1001);
    }
}

class BankAccount {
    private int balance = 0;

    void deposit(int amount) {
        this.balance += amount;
        System.out.println("Amount Deposited Successfully!");
    };

    void withdraw(int amount) {
        if (amount > this.balance) {
            System.out.println("Check  Your Current Balance!");
            return;
        }

        this.balance -= amount;
        System.out.println("Amount Deposited Successfully!");
    };
}
```

### 3. Inheritance:

    I. Create an Animal class with a method makeSound().
    II. Dog and Cat classes should inherit from Animal and implement their own versions of makeSound().
    III. Create objects of Dog and Cat and call their methods.

Ans -

```java

public class OOPS {
    public static void main(String[] args) {
        // Cat Object
        Cat c1 = new Cat();
        c1.makeSound();

        Dog d1 = new Dog();
        d1.makeSound();
    }
}

class Animal {
    void makeSound() {
        System.out.println("Animal is making a sound...");
    }
}

class Cat extends Animal {
    void makeSound() {
        System.out.println("Meow...");
    }
}

class Dog extends Animal {
    void makeSound() {
        System.out.println("Woof...");
    }
}
```

### Polymorphism

### 4. Make a Vehicle class with a method called move(). Then, make Car and Bike classes that inherit from Vehicle and have their own versions of the move() method. Create objects of both classes and call the move() method to see how polymorphism works.

Ans -

```java

public class OOPS {

    public static void main(String[] args) {
        Car c1 = new Car();
        c1.accelerate();

        Bike b1 = new Bike();
        b1.accelerate();
    }
}

class Vehicle {
    void accelerate() {
        System.out.println("Vehicle is accelerating...");
    }
}

class Car extends Vehicle {
    void accelerate() {
        System.out.println("Car is accelerating...");
    }
}

class Bike extends Vehicle {
    void accelerate() {
        System.out.println("Bike is accelerating...");
    }
}
```

### Intermediate Level Questions

### Method Overriding:

### 5. Create an Employee class with a method calculateSalary(). Manager and Developer classes should inherit from Employee and override calculateSalary(). Create objects and check which method is being called.

Ans -

```java

public class OOPS {

    public static void main(String[] args) {
        Developer dev1 = new Developer();
        dev1.calculateSalary();

        Manager man1 = new Manager();
        man1.calculateSalary();
    }
}

class Employee {
    void calculateSalary() {
        System.out.println("calculate the salary of employee");
    }
}

class Developer extends Employee {
    @Override
    void calculateSalary() {
        System.out.println("calculate the salary of Developer");
    }
}

class Manager extends Employee {
    @Override
    void calculateSalary() {
        System.out.println("calculate the salary of Manager");
    }
}
```

### 6. Constructor Overloading:

     Create a Person class that supports constructor overloading. One constructor should take only name, and another should take both name and age. Create objects and test both constructors.

Ans -

```java
public class OOPS {
    public static void main(String[] args) {
        Person arman = new Person("Armaan");
        System.out.println(arman.name + " " + arman.age);

        Person farman = new Person("Armaan", 18);
        System.out.println(farman.name + " " + farman.age);
    }
}

class Person {
    String name;
    int age;

    Person(String name) {
        this.name = name;
    }

    Person(String name, int age) {
        this.name = name;
        this.age = age;
    }
}
```

### 7. Static Methods and Properties:

    Create a MathUtils class with static methods add(a, b) and multiply(a, b). Add a static property PI and use it.

Ans -

```java
public class OOPS {

    public static void main(String[] args) {
        MathUtils.add(10, 20);
        MathUtils.multiply(2, 3);

        System.out.println(MathUtils.PI);
    }
}

class MathUtils {
    static float PI = 3.14f;

    static void add(int a, int b) {
        System.out.println(a + b);
    }

    static void multiply(int a, int b) {
        System.out.println(a * b);
    }
}
```

### Advanced Level Questions

### 8. Using Abstract Class:

Create an abstract class Vehicle with an abstract method startEngine(). Bike and Car should inherit from this class and implement their own versions of startEngine().

```java
public class OOPS {

    public static void main(String[] args) {
        Bike bike1 = new Bike();
        bike1.startEngine();

        Car car1 = new Car();
        car1.startEngine();
    }
}

abstract class Vehicle {
    abstract void startEngine();
}

class Bike extends Vehicle {
    void startEngine() {
        System.out.println("Bike's Engine Is Starting...");
    }
}

class Car extends Vehicle {
    void startEngine() {
        System.out.println("Car's Engine Is Starting...");
    }
}
```

### Using Interface:

### 9. Create a PaymentGateway interface with a method processPayment(amount). PayPal and Stripe classes should implement this interface and provide their own implementations.

### Singleton Pattern:

### 10. Create a DatabaseConnection class that maintains a single instance. Whenever getInstance() is called, it should return the same instance. These questions will help you strengthen your OOP concepts. Let me know if yo
