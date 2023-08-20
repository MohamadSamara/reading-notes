# Reading Notes: Understanding Java Concepts

**Difference Between Object and Class:**

In Java, all features, attributes, methods, etc. are linked to classes and objects. We cannot write a Java program just with the main function without declaring a class the way we can do in C++.

For example, if we want to write a program on a vehicle, a vehicle is a real-time object. But vehicles can be of various types. This means that the vehicle has a type attribute that can assume various values like the car, truck, scooter, bike, etc.

So the way we express the vehicle object in Java is we create a class “Vehicle” and then define its various attributes. Then we can declare various Vehicle class objects like car, bike, etc.

Inside the class, we can define the properties of Vehicle as the class attributes (data members) and methods like startVehicle (), stopVehicle (), etc.

This way, to express even the smallest of the entity in Java, we need to first identify the object and then define its blueprint or a class.

Summary : An **object** in Java is a tangible instance created from a **class**. A class defines the blueprint for an object, specifying its attributes (variables) and behaviors (methods). In simpler terms, if a class is a recipe, an object is the dish prepared using that recipe.

**Explaining Inheritance to a Non-Technical Friend:**

You know how in a family, certain traits, like curly hair or a friendly smile, can be passed down from parents to children? Well, in the world of programming, there's something similar called **inheritance**. Imagine you have a super talented artist parent who can paint amazing pictures. Now, instead of starting from scratch, you decide to become an artist too. With inheritance, you can actually "inherit" your parent's artistic skills and techniques, so you don't have to learn everything from the beginning.

So, in programming, a class is like a blueprint for creating objects with specific abilities. When one class "inherits" from another class, it's like saying, "Hey, I want to have all the cool things you can do, but I might add some of my own flair as well." Just like you inherit your parent's artistic talent and then put your own creative spin on it.

For example, let's say there's a class called "Animal" with basic features that all animals share, like moving and making sounds. Now, you want to create a specific animal, like a "Cat." Instead of writing all the basic stuff again, you can simply say that the "Cat" class inherits from the "Animal" class. This means the "Cat" class gets all the basic animal abilities, and you can focus on adding the unique qualities that make a cat special, like purring and chasing laser pointers.

So, inheritance is like getting a head start in programming by building on what already exists, just like how you build on your parent's talents to become an artist with your own creative style.

**Java Static Keyword:**

Static methods are also called class methods. It is because a static method belongs to the class rather than the object of a class.

And we can invoke static methods directly using the class name. For example,

```
class Test {
    // static method inside the Test class
    public static void method() {...}
}

class Main {
    // invoking the static method
    Test.method();
}
```

**Java Singleton Class:**

A **design pattern** is like a proven recipe for solving common programming problems. One such pattern is the **Singleton**. Imagine you have a magical wallet that only allows one coin inside. A **Singleton** class ensures there's only one instance of it throughout the program, which can be useful when you want to control access to shared resources, like a database connection.

**Factory pattern** is one of the most used design patterns in Java. This type of design pattern comes under creational pattern as this pattern provides one of the best ways to create an object.

In Factory pattern, we create object without exposing the creation logic to the client and refer to newly created object using a common interface.

**What is a Singleton:**

In object-oriented programming, a java singleton class is a class that can have only one object (an instance of the class) at a time. After the first time, if we try to instantiate the Java Singleton classes, the new variable also points to the first instance created. So whatever modifications we do to any variable inside the class through any instance, affects the variable of the single instance created and is visible if we access that variable through any variable of that class type defined.

## Things I Want to Know More About

-How can I effectively choose the right design pattern for a particular problem I'm trying to solve
