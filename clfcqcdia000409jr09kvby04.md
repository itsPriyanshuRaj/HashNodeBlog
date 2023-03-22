---
title: ""Mastering Abstraction in Java: How to Hide Implementation Details for Better Code Reusability""
seoTitle: "Mastering Abstraction in Object-Oriented Programming"
seoDescription: "Object Oriented Programming in Java language, it includes four pillars of oops Abstraction,Encapsulation,Polymorphism,Inheritance, Class,Objects, javascript"
datePublished: Fri Mar 17 2023 16:03:42 GMT+0000 (Coordinated Universal Time)
cuid: clfcqcdia000409jr09kvby04
slug: mastering-abstraction-in-java-how-to-hide-implementation-details-for-better-code-reusability
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1679068978245/6e7c0e1f-2132-43c0-a995-79d9f9b8cbad.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1679068841315/1c6c0494-921a-4658-b170-0c619a4999cf.png
tags: java, javascript, abstraction, 2articles1week

---

# Introduction

Object-oriented programming (OOP) is a popular programming paradigm used to design and develop software applications. One of the key features of OOP is an abstraction, which is the process of hiding the implementation details of a class from the user and providing only the essential information needed to use the class.

In Java, abstraction is achieved through the use of <mark>abstract classes and interfaces</mark>.

## Abstract Class

Abstract classes in Java are classes that cannot be instantiated, meaning that objects cannot be created from them. Instead, they serve as templates for other classes to inherit from. Abstract classes can contain both concrete and abstract methods. Concrete methods are methods that have an implementation, while abstract methods do not have an implementation and must be overridden by the classes that inherit from the abstract class.

Here's an example of an abstract class in Java:

```java
public abstract class Shape {
    public abstract double area();
    public abstract double perimeter();
}
```

In this example, the Shape class is abstract because it contains abstract methods (<mark>area() and perimeter(</mark>) ) that do not have an implementation.

### Let us take another example of an abstract class in Java:

```java
public class Circle extends Shape {
    private double radius;

    public Circle(double radius) {
        this.radius = radius;
    }

    public double area() {
        return Math.PI * radius * radius;
    }

    public double perimeter() {
        return 2 * Math.PI * radius;
    }
}
```

In this example, the Circle class inherits from the Shape class and provides implementations for the area() and perimeter() methods. Since the Shape class is abstract, objects cannot be created from it. However, objects can be created from the Circle class, which is a concrete class.

## Interfaces in Java (another way of achieving abstraction).

Interfaces in Java are another way to achieve abstraction.

An interface is a collection of abstract methods that are used to define a contract between a class and the outside world. Any class that implements an interface must provide an implementation for all of the methods defined in the interface.

Here's an example of an interface in Java:

```java
public class Book implements Printable {
    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public void print() {
        System.out.println("Book title: " + title);
        System.out.println("Book author: " + author);
    }
}
```

In this example, the Book class implements the Printable interface and provides an implementation for the print() method. Since the Printable interface contains only one method, any class that implements it must provide an implementation for that method.

# Conclusion

Abstraction is an important concept in Java and object-oriented programming in general. Abstraction allows programmers to create classes that are reusable and maintainable by hiding the implementation details of a class from the user and providing only the essential information needed to use the class.