# Reading Notes Class04 - Topic: OOP, Class, Object Binary, Decimal and Hexadecimal Numbers, and Constructor

## Introduction

In this module, we explore key concepts in Java programming, including object-oriented programming (OOP), classes, objects, binary, decimal, and hexadecimal numbers, as well as the significance of constructors. These topics are fundamental to building a strong foundation in Java development.

## Object-Oriented Programming (OOP) and Class

### Object vs. Class

- **Class:** A class is a blueprint or template for creating objects. It defines the structure and behavior that objects of that class will possess.

- **Object:** An object is an instance of a class, representing a tangible entity with specific attributes and behaviors.

### State and Behavior of a Student Object

Two types of state a Student object might have:

1. **Name:** Represents the student's name.
2. **Grades:** A collection of grades achieved by the student in different courses

Two types of behaviors a Student object might have:

1. **AttendClass:** Represents the student attending a class.
2. **CalculateGPA:** A method that calculates and returns the student's Grade Point Average (GPA)

### Constructor

The constructor is a special method that initializes an object when it's created. It ensures the object starts in a valid state.

Here are the keys to why constructors are significant:

1. **Object Initialization:** When an object is created using the `new` keyword, the constructor is automatically invoked. It is responsible for initializing the object's state, setting up initial values for its attributes or properties. This helps ensure that the object is in a valid and usable state right from the start.

2. **Parameterized Initialization:** Constructors can take parameters, allowing you to provide specific values or data during object creation. This enables you to customize the initial state of the object based on the values passed to the constructor.

3. **Code Reusability:** Constructors can be overloaded, meaning you can have multiple constructors with different parameter lists. This provides flexibility in object creation and allows you to reuse initialization logic by providing constructors that cater to various scenarios.

Declaration statement for a class named "Student":

```java
public class Student {
    // Fields
    // methods
    // constructor 
}
```

## Binary, Decimal, and Hexadecimal Numbers

### Number Representations

- **Binary:** Binary numbers are base-2 numbers, consisting of only 0s and 1s.

- **Decimal:** Decimal numbers are base-10 numbers, which we commonly use in everyday life.

- **Hexadecimal:** Hexadecimal numbers are base-16 numbers, using digits 0-9 and letters A-F.

<pre>Emaples :

1- The binary number 1101 is equivalent to the decimal number 13.

2- Converting the decimal number 52 to binary:

Divide 52 by 2: 52 / 2 = 26 (Remainder: 0)
Divide 26 by 2: 26 / 2 = 13 (Remainder: 0)
Divide 13 by 2: 13 / 2 = 6 (Remainder: 1)
Divide 6 by 2: 6 / 2 = 3 (Remainder: 0)
Divide 3 by 2: 3 / 2 = 1 (Remainder: 1)
Divide 1 by 2: 1 / 2 = 0 (Remainder: 1)
Reading the remainders from bottom to top, the binary representation of 52 is 110100.

3- Converting the decimal number 52 to hexadecimal:

Divide 52 by 16: 52 / 16 = 3 (Remainder: 4)
Divide 3 by 16: 3 / 16 = 0 (Remainder: 3)
The hexadecimal representation of 52 is 34.

</pre>

## Things I Want to Know More About

- How can we deal with these topic in industry world
