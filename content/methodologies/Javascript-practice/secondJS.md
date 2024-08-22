---
linkTitle: "Exercise 2"
title: Second Javascript exercise
weight: 2
---

{{< callout emoji="🎖️" >}}
Write a JavaScript program to create a class called 'Rectangle' with properties for width and height. Include two methods to calculate rectangle area and perimeter. Create an instance of the 'Rectangle' class and calculate its area and perimeter.
{{< /callout >}}
___

{{< tabs items="Explanation,Solution" >}}
  {{< tab >}}In the above exercise we create a "Person" class with properties for name, age, and country. It includes a method to display the person's details.\
  Finally it creates two instances of the Person class and displays their details using the displayDetails() method.{{< /tab >}}
  {{< tab >}}**Solution**:
  ```javascript
class Rectangle {
  constructor(width, height) {
    this.width = width;
    this.height = height;
  }

  calculateArea() {
    return this.width * this.height;
  }

  calculatePerimeter() {
    return 2 * (this.width + this.height);
  }
}

// Create an instance of the Rectangle class
const rectangle = new Rectangle(12, 10);

// Calculate area and perimeter of the rectangle
const area = rectangle.calculateArea();
const perimeter = rectangle.calculatePerimeter();

// Display the results
console.log(`Rectangle Area: ${area}`);
console.log(`Rectangle Perimeter: ${perimeter}`);
```

Sample output
```markdown
"Rectangle Area: 120"
"Rectangle Perimeter: 44"
```

  {{< /tab >}}

{{< /tabs >}}

___
Write your solution below

{{< codepen id="jYVvao" >}}

Solution in Codepen
{{< codepen id="yLQJLay" >}}