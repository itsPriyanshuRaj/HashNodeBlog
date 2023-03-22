---
title: "OOPs- An approach of thinking and writing code."
seoTitle: "Object Oriented Programming"
seoDescription: "Object Oriented Programming in Java language, it includes four pillars of oops Abstraction, Encapsulation, Polymorphism, Inheritance, Class, Objects"
datePublished: Thu Dec 22 2022 14:47:14 GMT+0000 (Coordinated Universal Time)
cuid: clbz76mtb000i08lb0xqe5z88
slug: oops-an-approach-of-thinking-and-writing-code
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1671719883023/kPbMB_CA0.png
tags: cpp, java, beginners, oops, object-oriented-programming

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1671717880125/uTc163GAz.png align="center")

**Object Oriented Programming or "OOPs"** is a computer programming design that models or organizes software design data or objects rather than functions and logic.

OOPs helps us structure our program very well. The main goal or aim of Object Oriented Programming is to write <mark>clean code.</mark>

It's is way to write **<mark>DRY</mark>** code**.**

### Let's understand the word Object Oriented.

It is a combination of two words **object and oriented**.

**Object** - An entity that exists in the real world that has unique attributes and behavior.

**Oriented** - Interested in a particular kind of entity or thing.

<mark>Now let's study the different pillars of OOPs.</mark>

# The Four Pillars of OOP

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1671718004801/y_jSDuf7W.png align="center")

## 1\. Abstraction

Abstraction is a process of <mark>hiding the implementation details </mark> and showing only important functions to the user.

It is a property by which only the essential details are displayed to the user. It helps programmer focus on what an object does instead of how it does.

*Examples -&gt; A man driving a Car. The man only knows that pressing the accelerator will increase the speed of a car but he does not know how the speed is actually increasing after pressing the accelerator.*

Abstraction is achieved in <mark>two ways</mark>:

*   Interface
    
*   Abstract Keywords
    

### Advantages of Abstraction

*   It reduces complexity.
    
*   Avoids code duplication.
    
*   It improves the modularity of an application.
    

# 2\. Encapsulation

Encapsulation is a process of wrapping code and data together into a single unit. It is also known **as data hiding.** Encapsulation can also be referred to as a protective shield that prevents the data from being accessed outside the shield.

<mark>Technically</mark>, the data is hidden from the class using the data hiding concept by making the class **Private**.

Encapsulation is achieved by declaring the variables in the class as **private** and writing methods in the class to set and get ( Using Getters and Setters) the values.

### Advantages of Encapsulation

*   Data Hiding.
    
*   Reusability.
    
*   Testing code is easy.
    

# 3\. Polymorphism

One of the most important features of OOPs.

Polymorphism is a combination of two Greek words, "<mark>Poly</mark>" and "<mark>Morphism</mark>". It allows us to perform any single action in different ways.

Example - A person can be an office employee, a customer, a singer etc.

Polymorphism is achieved using <mark>two ways</mark>.

*   **Compile time Polymorphism - It is the process of method overloading.**
    
*   **Runtime Polymorphism - It is the process of overriding a method (Re-declaring the method).**
    

### Difference between Overloading and Overriding

*   Overloading is basically the same method with different parameters.
    
*   Overriding is basically the same method with diffferne signatures or different body codes.
    

# 4\. Inheritance.

Inheritance is a mechanism by which one class is allowed to inherit the features of another class. In Java, inheritance means creating new classes based on existing ones. A class that inherits from another class can <mark>reuse</mark> the methods and fields of that class. In addition, you can add new fields and methods to your current class as well.  

<mark>Terminologies</mark> used in Inheritance.

*   **Super Class**: The class whose features are inherited also known as the Parent class.
    
*   **Sub Class**: The class that inherits the other class also known as the Child class.
    

The **extends keyword** is used for inheritance in java. Using the extends keyword indicates you are derived from an existing class. In other words, “extends” refers to increased functionality.

### Types of Inheritance.

1.  **Single Inheritance** - In Single Inheritance, the child class inherits the property of one parent class.
    
2.  **Multilevel Inheritance -** A derived class will be inheriting a base class, and as well as the derived class also acts as the base class for other classes.
    
3.  **Hierarchical Inheritance -** One class serves as a superclass for more than one class. <mark>(Not supported in Java)</mark>
    
4.  **Multiple Inheritance -** One class can have more than one superclass and inherit features from all parent classes. <mark>(Only achieved by Interface in Java).</mark>
    

## Conclusion

**Object-oriented programming revolves around the concepts of objects and classes**. In Java, the classes are referred to as templates for the objects while the objects are instances of a class so, the objects can inherit all the characteristics, variables, and functions of the class.