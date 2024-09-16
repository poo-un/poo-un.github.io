---
linkTitle: "Object"
title: Object concept
weight: 2
---

{{< callout type="info" >}}
In object-oriented programming (OOP), an <font color="#0047ab">object</font> is an instance of a <font color="#007bff">class</font>, encapsulating attributes and behaviors to model real-world entities.
{{< /callout >}}


Remember that we have a class called <font color="#007bff">`BankAccount`</font>. This class represents a bank account, and it has <font color="#F2613F">methods</font> to perform banking operations like depositing money and withdrawing money.

In our example, an object is an instance of the <font color="#007bff">`BankAccount`</font> class. Each individual bank account created from the <font color="#007bff">`BankAccount`</font> class is an object.

These objects, such as <font color="#007bff">`account1`</font> and <font color="#007bff">`account2`</font>, inherit <font color="#FFA600">attributes</font> and <font color="#F2613F">methods</font> from the class, but 
hold their own unique data.

#### Attributes:

  - Each bank account object has its own set of attributes that describe its specific state. For instance, each bank account object might have attributes like <font color="#FFA600">`accountNumber`</font>, <font color="#FFA600">`balance`</font>, and <font color="#FFA600">`accountHolder`</font>.

#### Methods:

  - Objects have access to the methods defined by their class. These methods define the behavior or actions that objects can perform. For example, each bank account object can use methods like <font color="#F2613F">`deposit`</font> and <font color="#F2613F">`withdraw`</font> to manage its funds.

#### Example:

Suppose we create two bank account objects from the <font color="#007bff">`BankAccount`</font> class:

| ㅤㅤㅤㅤㅤ<font color="#007bff">account1</font>ㅤㅤㅤㅤㅤ | ㅤㅤㅤㅤㅤ<font color="#007bff">account2</font>ㅤㅤㅤㅤㅤ |
|:--:|:--:|
| <font color="#FFA600">accountNumber</font>: 123456 <br/> <font color="#FFA600">balance</font>: 500 <br/> <font color="#FFA600">accountHolder</font>: John Doe | <font color="#FFA600">accountNumber</font>: 789012 <br/> <font color="#FFA600">balance</font>: 1000 <br/> <font color="#FFA600">accountHolder</font>: Jane Smith |
| <font color="#F2613F">deposit</font>(amount) <br/> <font color="#F2613F">withdraw</font>(amount) | <font color="#F2613F">deposit</font>(amount) <br/> <font color="#F2613F">withdraw</font>(amount) |

Each bank account object represents a distinct bank account with its own unique attributes and behaviors. For example, <font color="#007bff">`account1`</font> and <font color="#007bff">`account2`</font> have different <font color="#FFA600">`accountNumbers`</font>, <font color="#FFA600">`balances`</font>, and <font color="#FFA600">`accountHolders`</font>. They can each independently use the <font color="#F2613F">`deposit`</font> and <font color="#F2613F">`withdraw`</font> methods to manage their funds.

