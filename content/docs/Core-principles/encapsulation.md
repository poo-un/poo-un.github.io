---
linkTitle: "Encapsulation"
title: Encapsulation concept
weight: 1
---

{{< callout type="info" >}} <font color="#1E90FF">Encapsulation</font> is a fundamental principle of object-oriented programming (OOP) that restricts direct access to some of an object’s components and keeps data safe within objects. It is about bundling the data (<font color="#FFA600">attributes</font>) and the <font color="#F2613F">methods</font> that operate on that data into a single unit or class, while controlling access to the data through well-defined interfaces. {{< /callout >}}

<font color="#1E90FF">Encapsulation</font> allows the internal state of an <font color="#0047ab">object</font> be hidden from the outside world. External code cannot directly access or modify the <font color="#FFA600">attributes</font> of an <font color="#0047ab">object</font>; instead, interaction happens through <font color="#F2613F">public methods</font>, which manage how data is accessed and changed. This principle protects the integrity of the object and enforces a controlled interaction.

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
{{< callout >}}
The <font color="#FFA600">`accountNumber`</font>, <font color="#FFA600">`balance`</font>, and <font color="#FFA600">`accountHolder`</font> are private 🔒, meaning they cannot be accessed or modified directly from outside the class.
{{< /callout >}}

{{< callout >}}
The <font color="#F2613F">`deposit()`</font>, <font color="#F2613F">`withdraw()`</font>, and <font color="#F2613F">`getBalance()`</font> methods are public 🔓 and allow controlled interaction with the <font color="#007bff">`BankAccount`</font> class.
{{< /callout >}}


<font color="#1E90FF">Encapsulation</font> ensures that an object's internal state is protected from unintended interference, making it easier to maintain and modify code. It also improves the security and robustness of a program. 


#### Why Encapsulation Matters?

##### Data Integrity
By restricting direct access to <font color="#FFA600">attributes</font>, encapsulation helps ensure that the internal state of an object remains consistent. You can't set invalid or unsafe values on the <font color="#FFA600">`balance`</font> directly; instead, it’s modified through controlled <font color="#F2613F">methods</font> that validate input.

##### Modularity
<font color="#1E90FF">Encapsulation</font> allows changes to the internal implementation of a class without affecting how other parts of the code interact with it. For example, you can change how <font color="#F2613F">`getBalance()`</font> calculates the balance, and the external code won’t need to be updated.

##### Security
By keeping <font color="#FFA600">private attributes</font> inaccessible from outside, <font color="#1E90FF">encapsulation</font> enhances security. For example, it prevents unauthorized or unintended modifications to critical data, like changing an account’s balance directly.

##### Ease of Maintenance
<font color="#1E90FF">Encapsulation</font> makes the codebase easier to maintain. Changes to internal workings of the <font color="#0047ab">object</font> can be made without breaking the rest of the system since the external interface remains the same.

{{< callout type="info" >}}
**Next Step:**

Now that you’ve mastered how <font color="#1E90FF">encapsulation</font> protects object data and provides controlled access, proceed to learn about <font color="#32CD32">Abstraction</font>, which focuses on simplifying complex systems by hiding unnecessary details.
{{< /callout >}}