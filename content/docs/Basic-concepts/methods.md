---
linkTitle: "Methods"
title: Methods Concept
weight: 4
---

{{< callout type="info" >}}

In object-oriented programming, <font color="#F2613F">methods</font> define the actions that an object can perform. They are functions within a class that describe the behaviors or operations of the objects created from the class.
{{< /callout >}}

Methods are integral to how objects interact with each other and perform tasks. Let’s explore this concept using the <font color="#007bff">`BankAccount`</font> class example:

| ㅤㅤㅤㅤㅤ<font color="#007bff">BankAccount</font>ㅤㅤㅤㅤㅤ |
|:--:|
| <font color="#F2613F">deposit</font>(amount) <br/> <font color="#F2613F">withdraw</font>(amount) |

#### Bank Account Example:

For instance, let's use the <font color="#007bff">`BankAccount`</font> class to create two bank account objects:

| ㅤㅤㅤㅤㅤ<font color="#007bff">account1</font>ㅤㅤㅤㅤㅤ | ㅤㅤㅤㅤㅤ<font color="#007bff">account2</font>ㅤㅤㅤㅤㅤ |
|:--:|:--:|
| <font color="#FFA600">accountNumber</font>: 123456 <br/> <font color="#FFA600">balance</font>: 500 <br/> <font color="#FFA600">accountHolder</font>: John Doe | <font color="#FFA600">accountNumber</font>: 789012 <br/> <font color="#FFA600">balance</font>: 1000 <br/> <font color="#FFA600">accountHolder</font>: Jane Smith |
| <font color="#F2613F">deposit</font>(amount) <br/> <font color="#F2613F">withdraw</font>(amount) | <font color="#F2613F">deposit</font>(amount) <br/> <font color="#F2613F">withdraw</font>(amount) |

#### Method Usage:

- <font color="#007bff">`account1`</font> can use the <font color="#F2613F">`deposit`</font> method to add funds and the <font color="#F2613F">`withdraw`</font> method to withdraw funds.
- <font color="#007bff">`account2`</font> has the same methods but can perform <font color="#F2613F">`deposit`</font> and <font color="#F2613F">`withdraw`</font> operations based on its own balance and account details.

Each object has access to the same <font color="#F2613F">methods</font> defined in the class, which enables them to perform similar actions, but the outcomes of these methods depend on the object's specific attributes and current state.

{{< callout type="danger" >}}
Explore the **Core Principles** chapter to learn more about how methods integrate with the core principles of OOP, including inheritance, polymorphism, abstraction, and encapsulation.
{{< /callout >}}