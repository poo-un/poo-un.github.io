---
linkTitle: "Inheritance"
title: Inheritance concept
weight: 3
---

{{< callout type="info" >}}
<font color="#FF6347">Inheritance</font> is a fundamental principle of object-oriented programming (OOP) that allows a class (called a child or subclass) to inherit properties and behaviors from another class (called a parent or superclass). This enables code reusability, as common <font color="#FFA600">attributes</font> and <font color="#F2613F">methods</font> can be defined in the parent class and inherited by its subclasses.
{{< /callout >}}

<font color="#FF6347">Inheritance</font> promotes the reusability of code by allowing <font color="#007bff">classes</font> to derive common characteristics from a base class. It enables the creation of hierarchical relationships between <font color="#007bff">classes</font>, where a child class can inherit and extend the functionality of its parent class. Subclasses can override or extend inherited methods, adding flexibility and specificity.

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

{{< callout >}}
<font color="#007bff">`BankAccount`</font> provides shared <font color="#FFA600">attributes</font> like <font color="#FFA600">`accountNumber`</font>, <font color="#FFA600">`balance`</font>, and <font color="#FFA600">`accountHolder`</font>, along with shared <font color="#F2613F">methods</font> like <font color="#F2613F">`deposit()`</font>, <font color="#F2613F">`withdraw()`</font>, and <font color="#F2613F">`getBalance()`</font>.
{{< /callout >}}

{{< callout >}}
<font color="#007bff">`SavingsAccount`</font> inherits all the properties and behaviors of <font color="#007bff">`BankAccount`</font> but adds its own <font color="#FFA600">`interestRate`</font>🔒 attribute and the <font color="#F2613F">`applyInterest()`</font>🔓 method.
{{< /callout >}}

This example illustrates how <font color="#FF6347">Inheritance</font> allows new <font color="#007bff">classes</font> to build on top of existing ones. The <font color="#007bff">`SavingsAccount`</font> class can leverage all the functionality of <font color="#007bff">`BankAccount`</font> while introducing its own features like calculating interest. By sharing common code between the parent and child classes, inheritance reduces redundancy and promotes a cleaner design. 

#### Why Inheritance Matters?

##### Code Reusability
<font color="#FF6347">Inheritance</font> helps avoid duplication by allowing multiple subclasses to inherit common functionality from a single parent class. This way, shared <font color="#FFA600">attributes</font> and <font color="#F2613F">methods</font> can be reused without having to rewrite them in each subclass.

##### Extensibility
<font color="#FF6347">Inheritance</font> makes it easy to extend functionality. You can create new <font color="#007bff">classes</font> based on existing ones, introducing specialized behaviors while maintaining the foundational code from the parent class.

##### Maintainability
By organizing code into parent-child class relationships, <font color="#FF6347">Inheritance</font> simplifies maintenance. Changes in the parent class automatically propagate to all subclasses, ensuring consistency across your application.

##### Hierarchical Organization
<font color="#FF6347">Inheritance</font> naturally supports the creation of a class hierarchy. This makes it easier to understand and structure complex systems, particularly when there are multiple related <font color="#007bff">classes</font>.

{{< callout type="info" >}}
**Next Step:**

Now that you’ve learned how <font color="#FF6347">Inheritance</font> promotes code reusability and extensibility, the next step is to explore <font color="#8A2BE2">Polymorphism</font>, which allows objects of different classes to be treated uniformly.
{{< /callout >}}