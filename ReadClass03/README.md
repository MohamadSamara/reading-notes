# Reading Notes Class03 - Topic: Primitives And Objects , Exceptions , Scanner

## Introduction

The topic of Java programming concepts is crucial for understanding the fundamentals of Java and its application in software development. In this module, we delve into key concepts such as data types, exceptions, and input processing. These concepts form the building blocks of Java programming and provide a solid foundation for creating robust and efficient applications.

## Primitives vs. Objects

- **"int" vs. "Integer":** At the core, an `int` is a primitive data type, a fundamental building block representing whole numbers. In contrast, an `Integer` is an object that encapsulates an `int` and augments it with additional functionalities.

- **Default Values:** When uninitialized, an `int` defaults to `0`, while an `Integer` defaults to the `null` reference.

- **Autoboxing and Unboxing:**
The automatic transformation of a primitive type variable into its matching wrapper class object is known as autoboxing. When a primitive value is passed as a parameter to a function that expects a wrapper class object, the compiler automatically handles the conversion. It's assigned to a wrapper class type variable. The online Java compiler automatically converts between primitive types and the object wrapper classes that correspond to them. For example, it automatically converts from int to int, double to double, etc.

Unboxing is the process of automatically converting objects of wrapper classes to their corresponding primitives, for as Integer to int.

## Exceptions in Java

- Three basic categories of exceptions
  
  1. **Checked Exceptions:** These are exceptions that must be either caught or declared using the `throws` clause. They occur at compile-time and typically represent conditions that a well-written program can anticipate and recover from.

  2. **Unchecked Exceptions (Runtime Exceptions):** These exceptions are not required to be caught or declared. They occur during the execution of the program and usually signify unexpected conditions or programming errors that might not be recoverable.

  3. **Errors:** Errors are exceptional conditions that generally arise due to external factors beyond the control of the application, such as system failures or resource depletion. They are not expected to be handled within the application code.

## Statement for Exception Handling

- The `try-catch` statement is used to handle exceptions in Java. It consists of two main blocks:

  - **Try Block:** This block contains the code that might raise an exception. It's the portion of code where you expect a potential exception to occur.

  - **Catch Block(s):** These blocks follow the `try` block and specify how to handle different types of exceptions. If an exception occurs in the `try` block, the program will jump to the appropriate `catch` block to execute the corresponding error-handling code.

- The `throws` clause that is used to indicate that a method might throw certain types of exceptions. The `throws` clause is used in the method signature to declare the exceptions that the method might propagate, allowing the calling code to handle those exceptions.

```java
public void readFile(String filePath) throws FileNotFoundException, IOException {
    // Code that might throw FileNotFoundException or IOException
}
```

## Using Scanner to Read Text in Java

- Scanning text is useful for various tasks, such as parsing files, automation, data extraction, and quick processing of textual information, translating languages, managing inventory, analyzing data.

**Input from a Scanner Broken Down:**

Input from a `Scanner` in Java is broken down into tokens. A token is a sequence of characters that represents a unit of data. When you use a `Scanner` to read input, it breaks down the input stream into tokens based on delimiters, which are characters that separate tokens. By default, the delimiters are whitespace characters such as space, tab, and newline.

For example, let's say you use a `Scanner` to read a line of text: "apple orange banana"

When using whitespace as the delimiter, the input would be broken down into three tokens: "apple," "orange," and "banana."

`Tokenization` : The Scanner breaks input into tokens (words, numbers, symbols), enabling systematic processing.

This tokenization process allows you to process input data in manageable chunks, making it easier to analyze and work with different parts of the input.

## Things I Want to Know More About

- How can I choose between primitives and wrapper objects
