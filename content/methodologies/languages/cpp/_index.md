---
title: C++
prev: docs/
next: /morecontents
sidebar:
  open: true
---
# Object-oriented programming course


---
## Class and object
```c++
codepublic class GFG { 
      
    static String Employee_name; 
    static float Employee_salary; 
  
    static void set(String n, float p) { 
        Employee_name  = n; 
        Employee_salary  = p; 
    } 
  
    static void get() { 
        System.out.println("Employee name is: " +Employee_name ); 
        System.out.println("Employee CTC is: " + Employee_salary); 
    } 
  
    public static void main(String args[]) { 
        GFG.set("Rathod Avinash", 10000.0f); 
        GFG.get(); 
    } 
} 
```

- Output
```
Employee name is: Rathod Avinash
Employee CTC is: 10000.0
```
## Abstraction
Data Abstraction is the property by virtue of which only the essential details are displayed to the user. The trivial or non-essential units are not displayed to the user. Ex: A car is viewed as a car rather than its individual components.  
Data Abstraction may also be defined as the process of identifying only the required characteristics of an object, ignoring the irrelevant details. The properties and behaviors of an object differentiate it from other objects of similar type and also help in classifying/grouping the object.

```c++
//abstract class 
abstract class GFG{ 
  //abstract methods declaration 
  abstract void add(); 
  abstract void mul(); 
  abstract void div(); 
} 
```
## Encapsulation
It is defined as the wrapping up of data under a single unit. It is the mechanism that binds together the code and the data it manipulates. Another way to think about encapsulation is that it is a protective shield that prevents the data from being accessed by the code outside this shield.

```c++
//Encapsulation using private modifier  
//Employee class contains private data called employee id and employee name 
class Employee { 
    private int empid; 
      private String ename; 
} 
```

## Inheritance
Inheritance is an important pillar of OOP (Object Oriented Programming). It is the mechanism in Java by which one class is allowed to inherit the features (fields and methods) of another class. We are achieving inheritance by using ****extends**** keyword. Inheritance is also known as “****is-a****” relationship.

```c++
//base class or parent class or super class 
class A{ 
  //parent class methods 
  void method1(){} 
  void method2(){} 
} 
  
//derived class or child class or base class 
class B extends A{  //Inherits parent class methods 
  //child class methods 
  void method3(){} 
  void method4(){} 
}
```

## Example
```c++
// Java program to Demonstrate Polymorphism 
  
// This class will contain 
// 3 methods with same name, 
// yet the program will 
// compile & run successfully 
public class Sum { 
  
    // Overloaded sum(). 
    // This sum takes two int parameters 
    public int sum(int x, int y) 
    { 
        return (x + y); 
    } 
  
    // Overloaded sum(). 
    // This sum takes three int parameters 
    public int sum(int x, int y, int z) 
    { 
        return (x + y + z); 
    } 
  
    // Overloaded sum(). 
    // This sum takes two double parameters 
    public double sum(double x, double y) 
    { 
        return (x + y); 
    } 
  
    // Driver code 
    public static void main(String args[]) 
    { 
        Sum s = new Sum(); 
        System.out.println(s.sum(10, 20)); 
        System.out.println(s.sum(10, 20, 30)); 
        System.out.println(s.sum(10.5, 20.5)); 
    } 
} 
```
- Output
```
30
60
31.0
```
