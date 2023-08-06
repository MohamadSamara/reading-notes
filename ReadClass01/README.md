# Java Basics

- Variables
- Operators
- Expressions, Statements, and Blocks
- Control Flow Statements

## Variables

1- There are many kinds of variables in ``Java:``

2- Instance Variables ``(Non-Static)`` : declared without static keyword, these variables are unique for each instance of the class (each object)

3- Class Variables ``(Static)`` : declared with static keyword, meaning there is one copy of the variable regardless of how many instance have been created.

4- Local Variables : these variables are declared within the state of the object itself (Locally) and are only accessible to the methods and not the rest of the classes.

5- Parameters : variables accepted by a such as:

    public static void main (String[] args) // String[] args is considered a parameter

## Naming in Java

- Variables are case-sensitive.

- Variables name can have Letters,digits and two special characters ( _ and $ ).

- Names start with a letter,underscore or $ sign but can not start with a number.

- White space is not allowed

- Can not be a reserved keyword like ( int,String )

## What does “strong typed” mean?

    In Java, being "strongly typed" means that every variable and expression must have a specific data type, and the type is checked at compile-time. This ensures that the program is more robust and less prone to unexpected errors during runtime. By explicitly defining data types, Java enforces strict rules on variable assignments and operations, leading to safer and more predictable code.

## How many keywords does Java have?

    The Java programming language has 50 keywords. Each keyword has a specific meaning in the language. You can’t use a keyword for anything other than its pre-assigned meaning. Like (abstract , case , catch , default ...etc)

## Primitive Data Types in Java : Java has eight primitive data types that represent simple values

- byte
- short
- int
- long
- float
- double
- char
- boolean

### How do you print words to the console in Java?

     public class Main{
    public static void main(String[] args){
        String str = "Hello World"; 
        System.out.println(str); 
        }
    }
    // Output : Hello World

---

## Integers

### integers stores a real number , example

    public class Main{
    public static void main(String[] args){
        int val = 50 ; 
        System.out.println(val); 
        }
    }
    // Output : 50

## Float

### float stores a  decimals  number , example

    public class Main{
    public static void main(String[] args){
        int floatNumber = 5.75f; 
        System.out.println(floatNumber); 
        }
    }
    // Output : 5.75

## char

### char stores a charecter , example

    public class Main{
    public static void main(String[] args){
        char letter = 'h'; 
        System.out.println(letter); 
        }
    }
    // Output : h

## Boolean

### Boolean stores  true or false values

## Operators

| Operators      | Precedence |
| -----------    | ----------- |
| postfix        |expr++ expr--    |
| multiplicative | * / %        |
| additive       |   + -        |
|equality        | == !=        |
| AND            | &      |
| OR             | \|       |
| logical AND    | &&        |
| logical OR     | \|\|        |
| ternary        | ? :        |
| assignment     | = += -= *= /= %=       |

## Expressions, Statements, and Blocks

## Expressions :-

    public class Main{
    public static void main(String[] args){
        boolean flag = true ; 
        System.out.println(flag); 
        }
    }
    // Output : true 

### The expression ``` bool=true ``` returns an boolean because the assignment operator returns a value of the same data type as its left-hand operand;

## Statements

## Each statment followed by semicolon ```;```

## Blocks

## Block is group of statments between braces ``` {} ```

     public class Main{
        public static void main(String[] args){ // begin block 
        boolean bool = true ; 
        System.out.println(bool); 
        } // end block 
    }
    // Output : true

## Control Flow Statements

### The execution flow do the statment from top to bottom in your code but controle flow statment can change things some of this control flow statment :

- decision making (if-then, if-then-else, switch)
- looping statements (for, while, do-while)
- branching statements (break, continue, return)

## Explain to a non-technical friend the difference in how compilation works in Java and JavaScript

    When explaining the difference between compilation in Java and JavaScript to a non-technical friend, I would use the analogy of preparing a recipe. In Java, compilation is like preparing a recipe with clear instructions and precise measurements. The chef follows the recipe (Java code) step-by-step, ensuring each ingredient is accurately measured (strong typing), and the result is a fully prepared dish (compiled Java code) ready to be served (executed)

## Does code complining mean that it works correctly?

    Code compilation is an essential step in the software development process, but it does not guarantee that the code works correctly. Compilation checks for syntax errors and type compatibility, ensuring that the code meets the language's rules. However, it does not verify the logical correctness of the code or how it behaves during runtime. Correctly compiled code can still have logical errors, which may lead to unexpected behavior or undesired results when executed. To ensure that code works correctly, developers need to write comprehensive tests and perform thorough debugging

## Things I Want to Know More About

- Advanced concepts in Java, such as object-oriented programming, inheritance, and polymorphism
