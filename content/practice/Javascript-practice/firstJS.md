---
linkTitle: "Exercise 1"
title: First Javascript exercise
weight: 1
---

{{< callout emoji="🎖️" >}}
Write a JavaScript program to create a class called "Person" with properties for name, age and country. Include a method to display the person's details. Create two instances of the 'Person' class and display their details.
{{< /callout >}}
___
Plain code approach

{{< tabs items="Explanation,Solution" >}}
  {{< tab >}}In the above exercise we create a "Person" class with properties for name, age, and country. It includes a method to display the person's details.\
  Finally it creates two instances of the Person class and displays their details using the displayDetails() method.{{< /tab >}}
  {{< tab >}}**Solution**:
  ```javascript
class Person {
  constructor(name, age, country) {
    this.name = name;
    this.age = age;
    this.country = country;
  }

  displayDetails() {
    console.log(`Name: ${this.name}`);
    console.log(`Age: ${this.age}`);
    console.log(`Country: ${this.country}`);
  }
}

// Create instances of the Person class
const person1 = new Person('Francisca Rohan', 25, 'USA');
const person2 = new Person('Raimond Aruna', 30, 'Netherlands');

// Display details of person1
console.log('Person-1 Details:');
person1.displayDetails();

// Display details of person2
console.log('\nPerson-2 Details:');
person2.displayDetails();
```
Sample output
```markdown
"Person-1 Details:"
"Name: Francisca Rohan"
"Age: 25"
"Country: USA"
"
Person-2 Details:"
"Name: Raimond Aruna"
"Age: 30"
"Country: Netherlands"
```

  {{< /tab >}}

{{< /tabs >}}

___
Write your solution below

{{< codepen id="jYVvao" >}}

Solution in Codepen
{{< codepen id="xxQOxOq" >}}