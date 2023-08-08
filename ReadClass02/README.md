# Reading Class02 - Java Imports, Loops, and Arrays

## Java Imports

Understanding Java imports and built-in packages is crucial for effective coding in Java. It allows us to access pre-existing classes and functions that simplify the development process. This topic is essential as it forms the foundation of how we can leverage existing code to build more complex applications.

**Analogical Explanation:**
Built-in packages in Java are like a well-organized toolbox in a workshop. Just as different tools are neatly arranged in compartments for easy access, built-in packages contain classes and methods grouped by functionality. For instance, the `java.util` package is like a compartment filled with various utility tools to handle common tasks like managing collections or working with dates and times.

**Creating a New Package in IntelliJ:**
To create a new package in IntelliJ, follow these steps:

1. Right-click on the source folder (usually named "src") in the Project Explorer.
2. Select "New" and then choose "Package."
3. Enter the desired package name
4. Click "OK"

### Different Types of Loops in Java

Understanding loop types is fundamental in programming. They provide mechanisms for repetitive tasks and are used extensively in various applications.

**Loop Counter Loops:**

- `for` loop
- `while` loop
- `do-while` loop

**Difference Between While and Do-While Loops:**

- `while` loop: It checks the condition before executing the loop body. It might not run at all if the condition is initially false.
- `do-while` loop: It executes the loop body first and then checks the condition. It ensures that the loop body runs at least once, regardless of the initial condition.

## Java Arrays

Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.
To declare an array, define the variable type with square brackets:
    String[] cars;

We have now declared a variable that holds an array of strings. To insert values to it, we can use an array literal - place the values in a comma-separated list, inside curly braces:
    String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

**Three Built-In Methods for Arrays:**

1. `length`: Returns the number of elements in the array.
2. `sort`: Sorts the elements of the array in ascending order.
3. `toString`: Returns a string representation of the array.

**Determining the Size of an Array in Java:**
The size of an array in Java is determined when the array is created and remains fixed. It's specified within square brackets during declaration, indicating the number of elements the array can hold.

---

## Things I Want to Know More About

1. How do you handle situations where the size of an array needs to change dynamically?
