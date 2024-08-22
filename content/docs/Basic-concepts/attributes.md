---
linkTitle: "Attributes"
title: "Attributes concept"
weight: 3
---

{{< callout type="info" >}}
In object-oriented programming (OOP), an <font color="#FFA600">attribute</font> (also known as a property or field) is a characteristic or property of an object. It represents the data that an object holds and defines its state.
{{< /callout >}}

<font color="#FFA600">Attributes</font> are defined within a <font color="#007bff">class</font>, and each object created from that class has its own unique values for those attributes. For example, in a <font color="#007bff">`BankAccount`</font> class, attributes might include the <font color="#FFA600">account_number</font>, <font color="#FFA600">balance</font>, and <font color="#FFA600">account_holder</font>.

Let's delve into the concept of attributes considering the <font color="#007bff">`BankAccount`</font> class. Each bank account object created from this class will have its own set of attributes:

#### Example

Consider the <font color="#007bff">`BankAccount`</font> class. Each bank account object created from this class will have its own set of attributes:

|ㅤㅤㅤㅤㅤ<font color="#007bff">BankAccount</font>ㅤㅤㅤㅤㅤ|
|:--:|
| <font color="#FFA600">account_number</font>: Int <br/> <font color="#FFA600">balance</font>: Int <br/> <font color="#FFA600">account_holder</font>: String |

Suppose we create two <font color="#007bff">`BankAccount`</font> objects:

| ㅤㅤㅤㅤㅤ<font color="#007bff">Account 1</font>ㅤㅤㅤㅤㅤ | ㅤㅤㅤㅤㅤ<font color="#007bff">Account 2</font>ㅤㅤㅤㅤㅤ |
|:--:|:--:|
| <font color="#FFA600">account_number</font>: 123456 <br/> <font color="#FFA600">balance</font>: $500 <br/> <font color="#FFA600">account_holder</font>: John Doe | <font color="#FFA600">account_number</font>: 789012 <br/> <font color="#FFA600">balance</font>: $1000 <br/> <font color="#FFA600">account_holder</font>: Jane Smith |

In this example, we see that although both <font color="#007bff">`Account 1`</font> and <font color="#007bff">`Account 2`</font> are instances of the <font color="#007bff">`BankAccount`</font> class, each object has its own unique attribute values. 

Each object of the <font color="#007bff">`BankAccount`</font> class shares the same <font color="#FFA600">attributes</font>, but the values of these attributes differ from one object to another.
This distinction between objects is a fundamental concept in object-oriented programming, where each object carries its own specific data while sharing the same structure and behavior as defined by the class. Understanding how <font color="#FFA600">attributes</font> work helps in managing and manipulating objects effectively within a program.