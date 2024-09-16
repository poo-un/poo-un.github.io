---
linkTitle: "Inheritance"
title: Inheritance concept
weight: 3
---

{{< callout type="info" >}}
<font color="#FF6347">Inheritance</font> is a fundamental principle of object-oriented programming (OOP) that allows a class (called a child or subclass) to inherit properties and behaviors from another class (called a parent or superclass). This enables code reusability, as common <font color="#FFA600">attributes</font> and <font color="#F2613F">methods</font> can be defined in the parent class and inherited by its subclasses.
{{< /callout >}}

<font color="#FF6347">Inheritance</font> promotes the reusability of code by allowing <font color="#007bff">classes</font> to derive common characteristics from a base class. It enables the creation of hierarchical relationships between <font color="#007bff">classes</font>, where a child class can inherit and extend the functionality of its parent class.

#### Bank Account Example:

To illustrate <font color="#FF6347">Inheritance</font>, let’s extend our <font color="#007bff">`BankAccount`</font> class to create specialized types of accounts. For instance, we can create a <font color="#007bff">`SavingsAccount`</font> class that <font color="#FF6347">inherits</font> from <font color="#007bff">`BankAccount`</font> and adds a specific interest rate.

``` mermaid
classDiagram
class BankAccount {
  - Int accountNumber
  - Int balance 
  - String accountHolder
  + deposit(amount)
  + withdraw(amount)
  + getBalance()
}

class SavingsAccount {
  - Float interestRate
  + applyInterest()
}

BankAccount <|-- SavingsAccount
```

In this example, the <font color="#007bff">`SavingsAccount`</font> class inherits the <font color="#FFA600">`accountNumber`</font>, <font color="#FFA600">`balance`</font>, <font color="#FFA600">`accountHolder`</font> attributes, <font color="#F2613F">`deposit()`</font>, <font color="#F2613F">`withdraw()` </font> and <font color="#F2613F">`getBalance()` </font> methods from the <font color="#007bff">`BankAccount`</font> class. Additionally, it introduces its own attribute, <font color="#FFA600">`interestRate`</font>🔒, and the method <font color="#F2613F">`applyInterest()`</font>🔓.

<font color="#FF6347">Inheritance</font> allows us to define new <font color="#007bff">classes</font> based on existing ones, promoting reusability and reducing redundancy. By <font color="#FF6347">inheriting</font> from a parent <font color="#007bff">class</font>, subclasses can extend or modify the base functionality while sharing common behaviors. 

To continue your journey, let's explore the next core principle: <font color="#FFD700">Polymorphism</font>.