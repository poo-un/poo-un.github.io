---
linkTitle: "Object"
title: Object concept
weight: 2
---

In object-oriented programming (OOP), an <font color="#0047ab">object</font> is an instance of a <font color="#007bff">class</font>. It represents a real-world entity with its own set of properties (<font color="#FFA600">attributes</font>) and behaviors (<font color="#F2613F">methods</font>). <font color="#0047ab">Objects</font> are the building blocks of OOP and are used to model and interact with the system.

### Example: Bank Account Class

Remember that we have a class called <font color="#007bff">`BankAccount`</font>. This class represents a bank account, and it has <font color="#F2613F">methods</font> to perform banking operations like depositing money and withdrawing money.

In our example, an <font color="#0047ab">object</font> is an instance of the <font color="#007bff">`BankAccount`</font> class. Each individual bank account created from the <font color="#007bff">`BankAccount`</font> class is an <font color="#0047ab">object</font>.

- **Attributes**:
  - Each bank account object has its own set of attributes that describe its specific state. For instance, each bank account object might have attributes like <font color="#FFA600">`account_number`</font>, <font color="#FFA600">`balance`</font>, and <font color="#FFA600">`account_holder`</font>.

- **Methods**:
  - Objects have access to the methods defined by their class. These methods define the behavior or actions that objects can perform. For example, each bank account object can use methods like <font color="#F2613F">`deposit`</font> and <font color="#F2613F">`withdraw`</font> to manage its funds.

### Example:

Suppose we create two bank account <font color="#0047ab">objects</font> from the <font color="#007bff">`BankAccount`</font> class:

| ㅤㅤㅤㅤㅤ<font color="#007bff">Account 1</font>ㅤㅤㅤㅤㅤ | ㅤㅤㅤㅤㅤ<font color="#007bff">Account 2</font>ㅤㅤㅤㅤㅤ |
|:--:|:--:|
| <font color="#FFA600">account_number</font>: 123456 <br/> <font color="#FFA600">balance</font>: $500 <br/> <font color="#FFA600">account_holder</font>: John Doe | <font color="#FFA600">account_number</font>: 789012 <br/> <font color="#FFA600">balance</font>: $1000 <br/> <font color="#FFA600">account_holder</font>: Jane Smith |
| +<font color="#FF75A0">deposit</font>(amount) <br/> +<font color="#FF75A0">withdraw</font>(amount) | +<font color="#FF75A0">deposit</font>(amount) <br/> +<font color="#FF75A0">withdraw</font>(amount) |


Each bank account <font color="#0047ab">object</font> represents a distinct bank account with its own unique <font color="#FFA600">attributes</font> and behaviors. For example, <font color="#007bff">`Account 1`</font> and <font color="#007bff">`Account 2`</font> have different <font color="#007bff">`account numbers`</font>, <font color="#007bff">`balances`</font>, and <font color="#007bff">`account olders`</font>. They can each independently use the <font color="#F2613F">`deposit`</font> and <font color="#F2613F">`withdraw`</font> methods to manage their funds.

