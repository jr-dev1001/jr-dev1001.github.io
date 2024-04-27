---
layout: post
title: OOPS in Deep!
published: true
---
<h1 align="center">Hi <img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width="30px">, there! Let's Dive Deep into OOP with Java 🚀</h1>

“Everyone in this country should learn how to program because it teaches you how to think” – Steve Jobs
<div style="text-align:center;"> 
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e5/Steve_Jobs_WWDC07.jpg/1200px-Steve_Jobs_WWDC07.jpg" width=500px height=500px "alt="Steve Jobs">
</div>

# Overview

In our last blog post, we took a broad look at Object-Oriented Programming (OOP) and its significance. Now, we're going to roll up our sleeves and dive into each topic within OOP, using Java as our tool.

### Table of Contents:
1. Class
2. Object
3. Four pillars of OOPS
    - Encapsulation
    - Abstraction
    - Inheritence
    - Polymorphism

## Class: The Blueprint 📝

Think of a class as a blueprint or a recipe. It defines the structure and behavior of objects. Let's take a simple example: a `Car` class.

```java
public class Car {
    String make;
    String model;
    int year;

    public Car(String make, String model, int year) {
        this.make = make;
        this.model = model;
        this.year = year;
    }

    public void start() {
        System.out.println("The " + year + " " + make + " " + model + " is starting.");
    }
}
```

## Object: Bringing Classes to Life 🚗

An object is an instance of a class. It's like a physical manifestation of the blueprint. Let's create a `Car` object:

```java
public class Main {
    public static void main(String[] args) {
        Car myCar = new Car("Toyota", "Camry", 2022);
        myCar.start();
    }
}
```

## The Four Pillars of OOP

### Encapsulation: Wrapping It Up 🎁

Encapsulation is about bundling data (attributes) and methods (behaviors) within a single unit (class). It keeps data safe from outside interference. Here's a tweak to our `Car` class to demonstrate encapsulation:

```java
public class Car {
    private String make;
    private String model;
    private int year;

    // Constructor and methods remain the same...
}
```

### Abstraction: Focus on What Matters 🧠

Abstraction hides implementation details, showing only essential features. It allows us to work with high-level concepts. Let's abstract a method in our `Car` class:

```java
public abstract class Car {
    // Attributes and Constructor remain the same...

    public abstract void drive();
}
```

### Inheritance: Passing Down Knowledge 📚

Inheritance allows a new class (subclass) to inherit attributes and methods from an existing class (superclass). It promotes code reusability. Let's create an `ElectricCar` subclass:

```java
public class ElectricCar extends Car {
    private int batteryCapacity;

    // Constructor and additional methods...
}
```

### Polymorphism: Many Forms, One Concept 🔄

Polymorphism allows objects of different classes to be treated as objects of a common superclass. It enables methods to be implemented differently in derived classes. Let's override the `drive()` method in `ElectricCar`:

```java
public class ElectricCar extends Car {
    // Attributes, Constructor, and other methods...

    @Override
    public void drive() {
        System.out.println("The electric car is running silently.");
    }
}
```


And there you have it! We've explored the basics of OOP in Java. Keep experimenting and practicing to solidify your understanding. If you have any questions or topics you'd like us to delve into further, feel free to reach out! 🚀

#### sneak peak
In the next blog we will be learning `interfaces` in java.

