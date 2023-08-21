# Stacks And Queues

## What is a Stack?

In programming, a stack is an abstract, linear data type with a predefined capacity (or boundary). It follows a particular order for adding or removing elements. Linear data structures organize their components in a straight line, so if we add or remove an element, they will grow or shrink respectively.

Let us conceptualize stacks using a stack of plates placed in a box. The first plate placed in the stack (the plate at the bottom of the stack) will be the last one to be removed, and the plate added last would be the first to be removed.

This is called the Last In First Out (LIFO) or First In Last Out (FILO) ordering.

Stacks are used in a variety of ways when we code. We use stacks to implement functions, parsers, expression evaluation, and some algorithms. Stacks are great for processing nested structures, so they are important for understanding recursion.

A simple real-world application of a stack is reversing a string letter by letter. Another good example of a data stack is the undo and redo function on a computer or text editor. Undo removes your most recent change, and redo builds upon already existing changes.

### WHY Stacks

Stacks are perfect for situations where the order of items matters, like when you need to undo actions or evaluate expressions. They're like a stack of pancakes – you eat the top one first, and the last pancake you made is the first you eat.

### How do Stacks work?

The implementation of stacks is relatively easy. The functionality depends on the pop and push method, as you can see from the illustration above. The pop method removes or deletes elements from the stack, while the push method adds items to the stack.

When an element is inserted into a stack, it takes the top position and the variable storing this position points to the number below it. The top variable should be updated anytime an element is inserted or removed from it.

![Stack](stack.png)

## What is a Queue?

A queue is a lot like a stack. A Queue is also a linear structure that follows a First In First Out (FIFO) order, but they differ in how elements are removed. Queues are open from both ends: one end for inserting data (enqueue), and the other end for removing data (dequeue). A stack is only open from one end.

When it comes to queues, think of a check out counter at your favorite grocery store. The first person in the checkout line will be attended to first before others, and the last person in line will be attend to last. This is how a queue works. It has two ends, front and rear. Elements enter from the rear and leave from the front.

### Why Queues

Queues are used when tasks should be processed in the order they're received, such as printing documents or processing requests. They're like a line at the cafeteria – the person who arrives first gets served first.

### Types of Queues

There are three common types of queues you can expect to encounter. So far, we learned about the Linear Queue. The other two queues are:

Circular Queue: In a circular queue, the last element is connected to the first element to form a circle. Initially, the front and rear parts of the queue point to the same location, but they move apart as more elements are inserted into the queue. A real-life example of a circular queue is an automated traffic signal system.

Priority Queue: In priority queues, elements are sorted based on priority. The most important element appears first, and the least important appears last. Priority queues are used in operating systems for load balancing to determine which programs should be given more priority.

Essential Operations for Stacks & Queues

A typical stack must contain the following methods:

pop(): this method removes an element from the top of the stack and returns it.

push(): this method adds an element to the top of the stack.

A queue allows for the following operations:

enqueue(): this method adds an element to the end/rear of the queue

dequeue(): this method removes an element from the front of the queue

top(): returns the first element in the queue

initialize(): creates an empty queue

### How do Queue work?

The thing that makes queue different from stack is that a queue is open at both its ends. Hence, it follows FIFO (First-In-First-Out) structure, i.e. the data item inserted first will also be accessed first. The data is inserted into the queue through one end and deleted from it using the other end.

A real-world example of queue can be a single-lane one-way road, where the vehicle enters first, exits first. More real-world examples can be seen as queues at the ticket windows and bus-stops.

![Queue](Queue-in-DS-1.jpg)

### How to implement a Stack in Java

 ```java
  public static void main(String[] args) {
    //declaration of stack
    Stack<Integer> s = new Stack<>();

    //insert elements into stack
    s.push(10);
    s.push(20);
    s.push(30);

    //pop function returns and deletes thhe top element
    System.out.println(s.pop());

    //returning top element
    System.out.println(s.peek());

    //searching if an element exists
    System.out.println(s.search(20));

    //checks if stack is empty
    System.out.println(s.empty());



    //printing and deleting top element of stack
    while (!s.empty()) {
      System.out.println(s.peek());
      s.pop();
    }

  }
```

### How to implement a Queue in Java

 ```java
  public static void main(String[] args) {
        Queue<Integer> q1 = new LinkedList<Integer>();
        //Add elements to the Queue
        q1.add(10);
        q1.add(20);
        q1.add(30);
        q1.add(40);
        q1.add(50);
        System.out.println("Elements in Queue:"+q1);
        //remove () method =>removes first element from the queue
        System.out.println("Element removed from the queue: "+q1.remove());
        //element() => returns head of the queue
        System.out.println("Head of the queue: "+q1.element());
        //poll () => removes and returns the head
        System.out.println("Poll():Returned Head of the queue: "+q1.poll());
        //returns head of the queue
        System.out.println("peek():Head of the queue: "+q1.peek());
        //print the contents of the Queue
        System.out.println("Final Queue:"+q1);

  }
```

### Vocabulary

- LIFO: Last-In-First-Out
- FIFO: First-In-First-Out
- Data structure: A way to organize and store data
- Expression: A combination of values and operators

### Cheat Sheet

1. Stack (LIFO):
   - Add: push(item)
   - Remove: pop()

2. Queue (FIFO):
    - Add: enqueue(item)
    - Remove: dequeue()

### Quiz: Stacks and Queues

**Question 1:** Which data structure follows the Last-In-First-Out (LIFO) principle?
a) Queue
b) Stack
c) List
d) Array

**Question 2:** In a queue, which item do you remove first?
a) The item at the middle
b) The last item added
c) The item at the front
d) The smallest item

**Question 3:** When might you use a stack?
a) Processing items in the order they arrive
b) Managing a line of people
c) Evaluating expressions or undoing actions
d) Adding items to the back

**Question 4:** What is the main characteristic of a queue?
a) Last-In-First-Out (LIFO)
b) First-In-First-Out (FIFO)
c) Random order removal
d) Smallest-In-First-Out

**Answers:**

1. b) Stack
2. c) The item at the front
3. c) Evaluating expressions or undoing actions
4. b) First-In-First-Out (FIFO)
