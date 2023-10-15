# Read Class 19

**Define purely functional programming..**

Purely functional programming is a programming paradigm that treats all computation as the evaluation of mathematical functions. Purely functional programs do not have any side effects. This means that they do not modify any global state, such as global variables or files. Purely functional programs also do not perform any I/O operations.

**Can you change the state of a data structure using functional programming?**

Yes, you can change the state of a data structure using functional programming, but you must do so using pure functions. A pure function is a function that always returns the same output for the same input, and does not have any side effects. Side effects are changes to the state of the program outside of the function, such as modifying a global variable or writing to a file.

To change the state of a data structure using functional programming, you must create a new data structure that is a copy of the old data structure, with the desired changes made. This is known as **immutability**. Immutable data structures are data structures that cannot be modified once they are created.

For example, the following Java code shows how to change the state of a list using functional programming:

```java
import java.util.List;

public class Main {
    public static void main(String[] args) {
        List<Integer> myList = List.of(1, 2, 3);

        // Append 4 to the end of the list
        List<Integer> newList = myList.stream().collect(Collectors.toList());
        newList.add(4);

        // Reverse the list
        List<Integer> reversedList = myList.stream().reversed().collect(Collectors.toList());

        // Print the new list
        System.out.println(newList);

        // Print the reversed list
        System.out.println(reversedList);
    }
}
```

Output:

```java
[1, 2, 3, 4]
[3, 2, 1]
```

In this example, the `stream()` and `collect()` methods are both pure functions. They create new lists based on the input lists, but they do not modify the input lists themselves.

**How do you think purely functional programming will differ from the programs you’ve written so far in this course?**

Purely functional programming is a very different way of thinking about programming than the imperative programming paradigm that is most commonly used. In imperative programming, programs are written as a sequence of steps that modify the state of the program. In purely functional programming, programs are written as a set of functions that transform data.

One of the biggest differences between purely functional programming and imperative programming is the use of immutable data structures. In imperative programming, it is common to modify data structures in place. In purely functional programming, data structures are immutable, which means that they cannot be modified once they are created. This can make it more difficult to write purely functional programs, but it also makes them more predictable and easier to reason about.

Another difference between purely functional programming and imperative programming is the use of higher-order functions. Higher-order functions are functions that take other functions as arguments or return functions as results. Higher-order functions are very powerful and can be used to write very concise and expressive code.
