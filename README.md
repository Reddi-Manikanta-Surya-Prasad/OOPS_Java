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

## What is OOPS (Object-Oriented Programming)?  
OOPS is a programming paradigm based on real-world entities like **Bike, Car, ATM, etc.**  

---

## Procedural Programming vs. OOPS  

### **Procedural Programming**  
1. Programming is divided into functions.  
2. No proper data hiding; data moves freely and functions are prioritized.  
3. Overloading is not possible.  
4. Inheritance is not possible.  
5. Code reusability is not supported.  
**Examples:** Pascal, C, FORTRAN, etc.  

### **Object-Oriented Programming (OOPS)**  
1. Program is divided into **objects**.  
2. Objects provide **data hiding**, and data is given more importance than functions.  
3. Overloading is possible.  
4. Inheritance is supported.  
5. Code reusability is encouraged.  
**Examples:** Java, C++, Python, C#, etc.  

---

## Objects and Classes  

### **What is an Object?**  
An **Object** is an instance of a class that has:  
1. **Properties (States)** – e.g., Age, Color, Brand, Weight, etc.  
2. **Behaviors (Functions)** – e.g., Bark, Sleep, Drive, Apply Brakes, etc.  

### **Examples of Objects:**  
#### **Dog as an Object:**  
- **Properties:** Age, Breed, Color  
- **Behaviors:** Bark, Sleep, Eat  

#### **Car as an Object:**  
- **Properties:** Color, Type, Brand, Weight  
- **Behaviors:** Apply Brakes, Drive, Increase Speed  

---

## **Classes in Java**  
A **Class** is a blueprint from which objects are created. Multiple objects can be instantiated from a single class.  

### **Creating a Class in Java**  
```java
// Defining a class named Student
class Student {
    String name;
    int age;
    String address;

    // Functionality or Data Method
    void updateAddress(String newAddress) {
        this.address = newAddress;
    }
}

// Creating an Object of Student Class
Student engStudent = new Student();

```

# 1st Pillar of OOPS - Data Abstraction 
It hides the internal implementation and only shows essential functionality to the user.
It can be achieved through Interface and Abstract classes.
# Example:
Car - in car we can only see the break pedal, if we press that pedal then the speed of the car will be decreases.
Cellphone - how call is made that is Abstracted to us.

# Advantages of Abstraction
Increase security and confidentiality.
