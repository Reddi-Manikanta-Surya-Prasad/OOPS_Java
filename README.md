# OOPS in Java

## OOPS Fundamentals
- Overview of OOPS
- Objects and Classes

## Pillars of OOPS
1. **Data Abstraction**
2. **Encapsulation**
3. **Inheritance**
   - Types of Inheritance: Single, Multiple, etc.
4. **Polymorphism**
   - Static Polymorphism
   - Dynamic Polymorphism

## Relationships in OOPS
- **Is-a Relationship**
- **Has-a Relationship**

---

## What is OOPS (Object-Oriented Programming)?
OOPS is a programming paradigm based on the concept of objects, which represent real-world entities like a **Bike, Car, or ATM**.

---

## Procedural Programming vs. OOPS

### **Procedural Programming**
1. Programming is divided into parts called **functions**.
2. Does not provide proper data hiding; emphasizes functions over data.
3. Overloading is **not possible**.
4. Inheritance is **not possible**.
5. Code reusability is **not present**.

**Examples:** Pascal, C, FORTRAN, etc.

### **OOPS (Object-Oriented Programming)**
1. Program is divided into **objects**.
2. Objects provide **data hiding** and give importance to data.
3. Overloading is **possible**.
4. Inheritance is **possible**.
5. Code reusability is **present**.

**Examples:** Java, C++, Python, C#, etc.

---

## Objects and Classes

### **Objects Have Two Things:**
1. **Properties (States)** – e.g., Age, Color, Type.
2. **Behaviors (Functions/Methods)** – e.g., Barking, Sleeping, Driving.

### **Example of Objects**
- **Dog**: Properties - Age, Breed, Color; Behaviors - Bark, Sleep, Eat.
- **Car**: Properties - Color, Brand, Weight; Behaviors - Apply Brakes, Drive, Increase Speed.

### **Class and Object Creation**
A **class** is a blueprint/template to create objects. Multiple objects can be created from a single class.

```java
// Creating a class named Student
class Student {
    String name;
    int age;
    String address;
    
    // Method to update address
    void updateAddress(String newAddress) {
        this.address = newAddress;
    }
}

// Creating an object of Student class
Student engStudent = new Student();
```

---

## **1st Pillar of OOPS - Data Abstraction**
Data abstraction hides internal implementation details and only exposes essential functionalities.

### **Real-World Examples of Abstraction**
- **Car**: We press the brake pedal, but the internal mechanism of slowing down is hidden.
- **Cellphone**: We make a call, but the internal working of how a call is connected is abstracted.

### **Advantages of Abstraction**
- Increases **security** and **confidentiality**.
- Reduces complexity by hiding implementation details.

### **Implementation of Abstraction in Java**

```java
// Defining an interface
interface Car {
    void applyBrake();
}

// Implementing the interface
class CarImpl implements Car {
    public void applyBrake() {
        System.out.println("Brake applied!");
    }
}
```

