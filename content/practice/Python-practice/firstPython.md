---
linkTitle: "Exercise 1"
title: First Python exercise
weight: 1
---

{{< callout emoji="🎖️" >}}
Write a Python program to create a class representing a Circle. Include methods to calculate its area and perimeter.
{{< /callout >}}
___
Plain code approach

{{< tabs items="Explanation,Solution" >}}
  {{< tab >}}In the above exercise we create a "Person" class with properties for name, age, and country. It includes a method to display the person's details.\
  Finally it creates two instances of the Person class and displays their details using the displayDetails() method.{{< /tab >}}
  {{< tab >}}**Solution**:
  ```python
# Import the math module to access mathematical functions like pi
import math

# Define a class called Circle to represent a circle
class Circle:
    # Initialize the Circle object with a given radius
    def __init__(self, radius):
        self.radius = radius
    
    # Calculate and return the area of the circle using the formula: π * r^2
    def calculate_circle_area(self):
        return math.pi * self.radius**2
    
    # Calculate and return the perimeter (circumference) of the circle using the formula: 2π * r
    def calculate_circle_perimeter(self):
        return 2 * math.pi * self.radius

# Example usage
# Prompt the user to input the radius of the circle and convert it to a floating-point number
radius = float(input("Input the radius of the circle: "))

# Create a Circle object with the provided radius
circle = Circle(radius)

# Calculate the area of the circle using the calculate_circle_area method
area = circle.calculate_circle_area()

# Calculate the perimeter of the circle using the calculate_circle_perimeter method
perimeter = circle.calculate_circle_perimeter()

# Display the calculated area and perimeter of the circle
print("Area of the circle:", area)
print("Perimeter of the circle:", perimeter) 
```
Sample output
```markdown
Input the radius of the circle: 4
Area of the circle: 50.26548245743669
Perimeter of the circle: 25.132741228718345
```

  {{< /tab >}}

{{< /tabs >}}

___


