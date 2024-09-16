---
linkTitle: "Classes"
title: Class concept
weight: 1
---

{{< callout type="info" >}}
A class is a user-defined data type. A class is a blueprint for creating objects that share common properties and behaviors.
{{< /callout >}}

A <font color="#007bff">class</font> can be thought of as a blueprint that defines the structure of objects in a program. It's like a mold from which individual objects are created, each with its own attributes and behaviors.

Let's consider the concept of a class using the example of a <font color="#007bff">`BankAccount`</font>.

A <font color="#007bff">class</font> is like a blueprint or template for creating objects. In our example, the <font color="#007bff">`BankAccount`</font> class represents the blueprint for creating individual bank account objects.


``` mermaid
classDiagram
    class BankAccount {
    Int    accountNumber
    Int    Balance 
    String accountHolder
    deposit(amount)
    withdraw(amount)
    } 
```
<div style="display: flex; justify-content: center;">
    <div class="mermaid">
    classDiagram
    class BankAccount {
    Int    accountNumber
    Int    Balance 
    String accountHolder
    deposit(amount)
    withdraw(amount)
    } 
    </div>
</div>

|ㅤㅤㅤㅤㅤ<font color="#007bff">BankAccount</font>ㅤㅤㅤㅤㅤ|
|:--:|
| <font color="#FFA600">accountNumber </font>: Int <br/> <font color="#FFA600">balance </font>: Int<br/> <font color="#FFA600">accountHolder </font> : String |
| <font color="#F2613F">deposit</font>(amount) <br/> <font color="#F2613F">withdraw</font>(amount) |


#### Attributes:
  - <font color="#FFA600">Attributes</font> are characteristics or properties that describe the objects created from the class. For instance, in the case of a <font color="#007bff">`BankAccount`</font>, attributes could include <font color="#FFA600">`accountNumber`</font>, <font color="#FFA600">`balance`</font>, and <font color="#FFA600">`accountHolder`</font>.

#### Methods:
- <font color="#F2613F">Methods</font> are functions that define the behavior of the objects created from the class. In the context of a <font color="#007bff">`BankAccount`</font>, methods could include operations like <font color="#F2613F">`deposit`</font> and <font color="#F2613F">`withdraw`</font>, which specify how money can be added to or withdrawn from an account.


This class blueprint defines the structure for creating <font color="#007bff">`BankAccount`</font> objects. Each object instantiated from this class inherits <font color="#FFA600">attributes</font> such as <font color="#FFA600">`accountNumber`</font>, <font color="#FFA600">`balance`</font> and <font color="#FFA600">`accountHolder`</font>. Additionally, the <font color="#F2613F">methods</font> such as <font color="#F2613F">`deposit()`</font> and <font color="#F2613F">`withdraw()`</font>, enable the objects to perform operations like adding or withdrawing money.