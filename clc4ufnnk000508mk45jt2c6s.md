---
title: "Inheritance in Java: How it Works"
seoTitle: "Inheritance in Java: How it Works"
seoDescription: "object oriented programming concepts that includes inheritance, polymorphism, encapsulation and abstraction.
object oriented programming or oops in java"
datePublished: Mon Dec 26 2022 13:36:57 GMT+0000 (Coordinated Universal Time)
cuid: clc4ufnnk000508mk45jt2c6s
slug: inheritance-in-java-how-it-works
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1672061100727/b74bb9c5-7faf-46c0-9d63-40074260c481.jpeg
tags: programming-blogs, java, javascript, inheritance, object-oriented-programming

---

In the previous [<mark>blog</mark>](https://priyanshuraj.hashnode.dev/oops-an-approach-of-thinking-and-writing-code)<mark>,</mark> I wrote about Object Oriented Programming and its pillars. In this blog let's deep dive into one of the pillars of Object Oriented Programming called Inheritance.

## What is Inheritance?

A class that is derived from another class is called a *subclass* (also a *derived class*, *extended class*, or *child class*). The class from which the subclass is derived is called a *superclass* (also a *base class* or a *parent class*).

> The concept of Inheritance is powerful, when we create a new class and there is already a class that includes some code that we want, we can simply derive our new class from that existing class. We can reuse the existing method and fields without writing them again.

### Important Terminologies in Inheritance.

1. **Class:** A template or blueprint on which objects are created.
    
2. **Super Class/ Parent Class:** The class whose properties are inherited is known as a superclass.
    
3. **Sub Class/ Child Class:** The class that inherits the property of the parent/other class is known as Child Class.
    

## How to use Inheritance?

We use the <mark>extends keyword</mark>. Using the extends keyword indicates we are derived from an existing class.

```java
//SYNTAX 
class derived-class extends base-class{
    //methods and fields
}
```

### Example of Inheritance

In the below example of inheritance, the class Employee is a base class, class Engineer is a derived class that extends the Employee class Test is a driver class to run the program.

```java
//Java program to show how illustration works.
//Code Reference - GeekforGeeks
class Employee{ //Base class or Super Class
    int salary = 20000;
}

//Subclass
class Engineer extends Employee{
    int benefits = 10000;
}

//Derive class
class Test{
    public static void main(String[] args){
        Engineer e1 = new Engineer();
        System.out.println("Salary :" +e1.salary + "and Benefits " + e1.benefits);
    }
}
```

```java
//Output
Salary: 20000
Benefits: 1000
```

## Types of Inheritance

1. **Single Inheritance** - In single Inheritance, the subclass inherits the features of one superclass.
    
    ```java
    //Example of Single Inheritance
    class Animal{  // Parent class or Superclass
        void eat(){
            System.out.println("Eating");
        }
    }
    class Dog extends Animal{ //Subclass or child class
        void bark(){
            System.out.prinltln("Barking");
        }
    }
    class Test{
        public static void main(String args[]){
            Dog obj = new Dog();  //Creating object of child class
            obj.bark();
            obj.eat();
        }
    }
    ```
    
    ```java
    //Output
    Barking...
    Eating...
    ```
    
2. **Multilevel Inheritance -** In Multilevel inheritance, a derived class inherits a base class and the respective derived class also acts as the base class for other classes.
    

```java
//Example of Multilevel Inheritance
class Animal{  // Parent class or Superclass
    void eat(){
        System.out.println("Eating");
    }
}
class Dog extends Animal{ //Subclass or child class
    void bark(){
        System.out.prinltln("Barking");
    }
}
//BabyDog class inherits the Dog class which again inherits the Animal Class. (Multilevel Inheritance)
class BabyDog extends Dog{
    void weep(){
        System.out.println("Weeping");
    }
}

class Test{  
    public static void main(String args[]){  
        BabyDog obj = new BabyDog();  
        obj.weep();  
        obj.bark();  
        obj.eat();  
    }
}  
```

```java
//Output
weeping...
barking...
eating...
```

1. **Multiple Inheritance -** In Multiple Inheritance, one class can have more than one superclass(Parent Class) and inherit properties from all parent classes. <mark> It is achieved only through Interfaces in Java.</mark>
    
    ```java
    //Example of Multiple Inheritance
    //Code Refrence - GeekforGeeks
    interface one {
        public void print_geek();
    }
     
    interface two {
        public void print_for();
    }
     
    interface three extends one, two {
        public void print_geek();
    }
    class child implements three {
        @Override public void print_geek()
        {
            System.out.println("Geeks");
        }
     
        public void print_for() { System.out.println("for"); }
    }
     
    // Drived class
    public class Main {
        public static void main(String[] args)
        {
            child c = new child();
            c.print_geek();
            c.print_for();
            c.print_geek();
        }
    }
    ```
    

```java
//Output
Geeks
for
Geeks
```

## What can be Inherited?

* All <mark>protected</mark> and <mark>public</mark> fields and methods from parents' class.
    

## What can not be Inherited?

* Private method and fields
    
* Constructors
    
* Multiple classes. Java supports only **single inheritance**.
    
* Fields. Individual fields of a class cannot be overridden by the subclass.
    

<mark>That's all about the Inheritance in Java. Do leave any feedback if you have.</mark>