---
linkTitle: "Encapsulation"
title: Encapsulation concept
weight: 1
---

{{< callout type="info" >}} <font color="#1E90FF">Encapsulation</font> is a fundamental principle of object-oriented programming (OOP) that restricts direct access to some of an object’s components and keeps data safe within objects. It is about bundling the data (<font color="#FFA600">attributes</font>) and the <font color="#F2613F">methods</font> that operate on that data into a single unit or class, while controlling access to the data through well-defined interfaces. {{< /callout >}}

<font color="#1E90FF">Encapsulation</font> helps to safeguard an object’s state by providing controlled access to its <font color="#FFA600">attributes</font> through public <font color="#F2613F">methods</font>. This principle allows for hiding the internal workings of an <font color="#0047ab">object</font> and exposing only what is necessary for other <font color="#0047ab">objects</font> or code to interact with it.

#### Bank Account Example:

To demonstrate this principle, let’s revisit the <font color="#007bff">`BankAccount`</font> class. We will use <font color="#1E90FF">encapsulation</font> to restrict direct access to the <font color="#FFA600">`account attributes`</font> and allow interactions only through the <font color="#F2613F">`deposit()`</font> and <font color="#F2613F">`withdraw()`</font> methods:

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
The attributes <font color="#FFA600">`accountNumber`</font>, <font color="#FFA600">`balance`</font>, and <font color="#FFA600">`accountHolder`</font> are `private` 🔒 (denoted by the `-` symbol) and cannot be accessed directly.
Methods like <font color="#F2613F">`deposit(amount)`</font>, <font color="#F2613F">`withdraw(amount)`</font>, and <font color="#F2613F">`getBalance()`</font> are `public` 🔓 (denoted by the `+` symbol) and provide controlled access to the account’s data.

<font color="#1E90FF">Encapsulation</font> ensures that an object's internal state is protected from unintended interference, making it easier to maintain and modify code. It also improves the security and robustness of a program. 

Now that you have a solid understanding of <font color="#1E90FF">encapsulation</font>, let’s continue to explore the next core principle: <font color="#32CD32">Abstraction</font>.