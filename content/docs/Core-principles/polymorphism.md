---
linkTitle: "Polymorphism"
title: Polymorphism concept
weight: 4
---

{{< callout type="info" >}} <font color="#8A2BE2">Polymorphism</font> is a fundamental principle in OOP that allows objects of different classes to be treated as objects of a common base class. It enables one interface to be used for different data types or classes, simplifying code and making it more flexible. {{< /callout >}}

<font color="#8A2BE2">Polymorphism</font> allows for methods to behave differently based on the object that invokes them. It enables multiple classes to implement methods that share the same name but provide different functionalities depending on the specific class.

For example, a banking system might have different types of accounts such as <font color="#007bff">`SavingsAccount`</font> and <font color="#007bff">`CheckingAccount`</font>. Both types of accounts could share a common method like <font color="#F2613F">`applyInterest()` </font>, but each would calculate interest in a different way.

#### Bank Account Example:

Imagine we have a base class, <font color="#007bff">`BankAccount`</font>, and a subclass, <font color="#007bff">`SavingsAccount`</font>. The method <font color="#F2613F">`applyInterest()`</font> behaves differently in the <font color="#007bff">`SavingsAccount`</font> class compared to a more generic method in <font color="#007bff">`BankAccount`</font>:


``` mermaid
classDiagram
class BankAccount {
  + deposit(amount)
  + withdraw(amount)
  + getBalance()
} 

class SavingsAccount {
  + Float interestRate
  + applyInterest()
  + withdraw(amount)
}

BankAccount <|-- SavingsAccount
```

{{< callout >}}
In the diagram:

The method <font color="#F2613F">`withdraw(amount)`</font> is <font color="#8A2BE2">overridden</font> in the <font color="#007bff">`SavingsAccount`</font> class to account for savings-specific rules (like a fee or limit).
Methods within the same class that share the same name but have different parameters.

The method <font color="#F2613F">`applyInterest()`</font> adds behavior specific to savings accounts, demonstrating <font color="#8A2BE2">method overloading</font> because a subclass is providing specific implementation of a method already defined in its superclass.
{{< /callout >}}

<font color="#8A2BE2">Polymorphism</font> allows <font color="#007bff">`BankAccount`</font> and <font color="#007bff">`SavingsAccount`</font> to share similar methods, but execute them differently depending on the object’s type. For example, both classes have a <font color="#F2613F">`withdraw(amount)`</font> method, but the behavior differs depending on whether the object is a <font color="#007bff">`BankAccount`</font> or a <font color="#007bff">`SavingsAccount`</font>.

#### Why Polymorphism Matters?

##### Code Reusability
<font color="#8A2BE2">Polymorphism</font> allows a base class like <font color="#007bff">`BankAccount`</font> to define general behavior, while subclasses like <font color="#007bff">`SavingsAccount`</font> can build on and modify that behavior. This makes it easier to extend the system without rewriting code.

##### Maintainability
<font color="#8A2BE2">Polymorphism</font> simplifies code maintenance. If you need to change the behavior of a method for a particular <font color="#007bff">class</font>, you can override it in the subclass, without altering the base class or other subclasses.

##### Dynamic Behavior
At runtime, the system can decide which <font color="#F2613F">method</font> to invoke depending on the object's type, leading to more flexible and dynamic code.

{{< callout type="info" >}}
**Next Step:**

Now that you’ve mastered all four core principles of object-oriented programming (OOP), it’s time to explore the [Methodologies](/content/methodologies/_index.md) section, where you can dive into different learning paths. These methodologies provide various ways to apply the OOP concepts you’ve learned based on different teaching styles and use cases.
{{< /callout >}}

### Quiz
---

<form id="quiz">
  <label>Question 1: What is OOP?</label><br>
  <input type="radio" name="q1" value="a"> A programming paradigm<br>
  <input type="radio" name="q1" value="b"> A database model<br>
  <input type="submit" value="Submit">
</form>
<div id="result"></div>

<script>
  document.getElementById('quiz').onsubmit = function(e) {
    e.preventDefault();
    const answer = document.querySelector('input[name="q1"]:checked').value;
    document.getElementById('result').innerText = answer === 'a' ? 'Correct!' : 'Try again!';
  };
</script>