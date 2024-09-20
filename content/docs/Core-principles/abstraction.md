---
linkTitle: "Abstraction"
title: Abstraction concept
weight: 2
---

{{< callout type="info" >}} <font color="#32CD32">Abstraction</font> is a core principle of object-oriented programming (OOP) that focuses on hiding complex implementation details and exposing only the essential features of an <font color="#0047ab">object</font>. By using abstraction, developers can simplify complex systems by breaking them down into more manageable parts. {{< /callout >}}

In OOP, <font color="#32CD32">Abstraction</font> enables you to represent essential aspects of an <font color="#0047ab">object</font> without exposing its internal workings. It allows for designing classes that can interact with other parts of the system while hiding unnecessary complexities.

For example, in a banking application, you might need to interact with <font color="#007bff">bank accounts</font>, but you don’t need to know the complex algorithms that calculate interest or handle transactions. Instead, you only care about the essential methods and attributes like <font color="#F2613F">`deposit()`</font>, <font color="#F2613F">`withdraw()`</font>, and <font color="#FFA600">`balance`</font>.

#### Bank Account Example

Let’s <font color="#32CD32">abstract</font> the core functionality of a bank account by defining a <font color="#007bff">`BankAccount`</font> class that hides the internal logic while exposing essential <font color="#F2613F">methods</font> for interacting with it.

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
```

{{< callout >}} Attributes (<font color="#FFA600">`accountNumber`</font>, <font color="#FFA600">`balance`</font>, and <font color="#FFA600">`accountHolder`</font>) are `private` 🔒
{{< /callout >}}

These represent the internal data of the <font color="#007bff">`BankAccount`</font>. By keeping these attributes `private`, we ensure that they cannot be accessed or modified directly by external code.
For example,  without abstraction, an external user could directly modify attributes like <font color="#FFA600">`balance`</font> to any value, even negative amounts. 

<font color="#32CD32">Abstraction</font> protects this data, ensuring that changes are made through controlled methods like <font color="#F2613F">`deposit(amount)`</font> and <font color="#F2613F">`withdraw(amount)`</font>. 

{{< callout >}} Methods like <font color="#F2613F">`deposit(amount)`</font> and <font color="#F2613F">`withdraw(amount)`</font> are `public` 🔓 {{< /callout >}} 

These methods provide an interface to interact with the <font color="#007bff">`BankAccount`</font> object. Through abstraction, users can perform essential operations without needing to know how these methods are implemented internally.

#### Why Abstraction Matters?

##### Separation of Concerns

<font color="#32CD32">Abstraction</font> ensures that each part of the system focuses on a specific task. The <font color="#007bff">`BankAccount`</font> class manages the account data internally, while external code only interacts with it through public methods. This separation makes the system easier to understand, maintain, and extend.

##### Security

By hiding the internal state of the object, we prevent unauthorized or unintended changes. For instance, without abstraction, a user could directly change the <font color="#FFA600">`accountNumber`</font> of an account. <font color="#32CD32">Abstraction</font> ensures that such sensitive data is protected, allowing only authorized interactions through the defined methods.

##### Simplified Interface

Users of the class only need to focus on what’s essential for them. A person using the <font color="#007bff">`BankAccount`</font> class doesn't care about how the balance is stored in memory or how funds are transferred; they only care about interacting with the interface provided—depositing, withdrawing, and checking the balance.

Through <font color="#32CD32">Abstraction</font>, we define a simple interface for interacting with objects, hiding unnecessary details while maintaining control over how data is accessed and modified. This principle enhances security, improves code maintainability, and ensures a cleaner, more understandable interface.

{{< callout type="info" >}}
**Next Step:** 

Now that you’ve seen how <font color="#32CD32">abstraction</font> simplifies object interactions, explore <font color="#FF6347">Inheritance</font> , which allows a class (called a child or subclass) to inherit properties and behaviors from another class (called a parent or superclass).
{{< /callout >}}
