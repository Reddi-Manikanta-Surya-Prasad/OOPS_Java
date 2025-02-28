# OOPS in Java

## OOPS Fundamentals:
- Overview of OOPS
- Objects and Classes

## Pillars of OOPS:
### 1. Data Abstraction
### 2. Encapsulation
### 3. Inheritance
   - Types of Inheritance: Single, Multiple, etc.
### 4. Polymorphism
   - Static Polymorphism
   - Dynamic Polymorphism

## Relationships in OOPS:
- **Is-a Relationship**
- **Has-a Relationship**

## What is OOPS? (Object-Oriented Programming)
OOPS is a programming paradigm based on objects, which are instances of classes. An object represents a real-world entity like a **Bike, Car, ATM, etc.**

## Procedural Programming vs. OOPS

### Procedural Programming:
1. Programming is divided into parts called functions.
2. Does not provide proper data hiding, focuses on functions, and allows data to move freely.
3. Overloading is not possible.
4. Inheritance is not possible.
5. Code reusability is limited.

**Examples:** PASCAL, C, FORTRAN, etc.

### OOPS:
1. Programming is divided into objects.
2. Objects provide data hiding and focus on data.
3. Overloading is possible.
4. Inheritance is possible.
5. Code reusability is a key feature.

**Examples:** Java, C++, Python, C#, etc.

---
## Objects and Classes
### Objects have two components:
1. **Properties (States)** – e.g., Age, Color, Type, Weight, etc.
2. **Behavior (Functions/Methods)** – e.g., Bark, Sleep, Eat, Drive, Apply Brakes, etc.

### Example:
- **Dog** (Object)
  - **Properties:** Age, Breed, Color, etc.
  - **Behaviors:** Bark, Sleep, Eat, etc.

- **Car** (Object)
  - **Properties:** Color, Type, Brand, Weight, etc.
  - **Behaviors:** Apply Brakes, Drive, Increase Speed, etc.

### Class:
A **class** is a template or blueprint from which objects are created. From one class, we can create multiple objects.

**Syntax to define a class in Java:**
```java
class Student {
    String name;
    int age;
    String address;
}
```

### Creating an Object:
```java
Student engStudent = new Student();
```

---
## 1st Pillar of OOPS - Data Abstraction
Data Abstraction hides the internal implementation and only shows essential functionality to the user.

### Example:
- **Car** – We only see the brake pedal. Pressing it decreases the car's speed, but the internal mechanism is hidden.
- **Cell Phone** – How a call is made is abstracted from the user.

### Advantages of Abstraction:
- Increases security and confidentiality.

**Java Example of Abstraction:**
```java
interface Car {
    void applyBrake();
}

class CarImpl implements Car {
    public void applyBrake() {
        System.out.println("Brakes Applied!");
    }
}
```

---
## 2nd Pillar of OOPS - Data Encapsulation
Encapsulation bundles data and the code that manipulates the data into a single unit. It is also known as **Data Hiding**.

### Steps to Achieve Encapsulation:
1. Declare class variables as **private**.
2. Provide **public** getter and setter methods to access and modify variables.

### Advantages of Encapsulation:
- Loosely coupled code.
- Better access control and security.

**Java Example of Encapsulation:**
```java
class Student {
    private String name;
    private int age;
    
    // Getter method
    public String getName() {
        return name;
    }
    
    // Setter method
    public void setName(String name) {
        this.name = name;
    }
}
```


