# Read Class 30 - Hash Tables

**WHAT is a hash table?**

A hash table is an array of buckets, where each bucket contains a linked list of key-value pairs. The key is used to compute the index of the bucket where the value is stored. This is done using a hash function, which is a function that takes a key and returns an integer value.

**WHY do we use hash tables?**

Hash tables are a very efficient data structure for storing and retrieving key-value pairs. They allow us to find the value associated with a key in constant time, on average. This is much faster than other data structures, such as linked lists or arrays, which can take linear time to search.

**HOW does a hash table work?**

To insert a new key-value pair into a hash table, we first compute the index of the bucket where the value should be stored. This is done by applying the hash function to the key. We then add the key-value pair to the linked list in the corresponding bucket.

To retrieve the value associated with a key, we first compute the index of the bucket where the value should be stored. We then search the linked list in the corresponding bucket for the key. If the key is found, we return the associated value. If the key is not found, we return null.

Here is a simple example of how to use a hash table to store the names and phone numbers of people:

```java
public class HashTable<K, V> {

    private Node<K, V>[] buckets;
    private int size;

    public HashTable() {
        this.buckets = new Node[100];
        this.size = 0;
    }

    public void put(K key, V value) {
        int index = hash(key) % buckets.length;

        Node<K, V> node = new Node<>(key, value);
        Node<K, V> currentNode = buckets[index];

        while (currentNode != null) {
            if (currentNode.key.equals(key)) {
                currentNode.value = value;
                return;
            }

            currentNode = currentNode.next;
        }

        node.next = buckets[index];
        buckets[index] = node;
        size++;
    }

    public V get(K key) {
        int index = hash(key) % buckets.length;

        Node<K, V> currentNode = buckets[index];

        while (currentNode != null) {
            if (currentNode.key.equals(key)) {
                return currentNode.value;
            }

            currentNode = currentNode.next;
        }

        return null;
    }

    private int hash(K key) {
        return key.hashCode();
    }

    private static class Node<K, V> {
        private K key;
        private V value;
        private Node<K, V> next;

        public Node(K key, V value) {
            this.key = key;
            this.value = value;
            this.next = null;
        }
    }
}
```

To use the hash table, simply instantiate a new HashTable object and then call the put() and get() methods to add and retrieve key-value pairs. For example:

```java
HashTable<String, Integer> hashTable = new HashTable<>();

// Add some key-value pairs
hashTable.put("Mohamad", 1234567890);
hashTable.put("Samara", 9876543210);

// Get the value associated with a key
int phoneNumber = hashTable.get("Mohamad");

System.out.println(phoneNumber);
```

Output:

```java
1234567890
```

Hash tables are a very powerful data structure that can be used to implement a wide variety of algorithms and applications. They are particularly well-suited for applications where speed is important, such as caching and database indexing.

## Advantages of Hash Tables

Hash tables have several advantages. First, they are very fast for searching and insertion. Second, they are very scalable. As you add more data to a hash table, you can simply increase the size of the hash table.

## Disadvantages of Hash Tables

Hash tables also have some disadvantages. First, they can be inefficient if there are many collisions. Second, they can be memory-intensive, especially if the hash table is very large.

## Tutorial / walk through an example

### Tutorial

1. Create a new hash table object.
2. To add a new key-value pair to the hash table, call the `put()` method. The `put()` method takes two arguments: the key and the value.
3. To retrieve the value associated with a key, call the `get()` method. The `get()` method takes one argument: the key.
4. To check if the hash table contains a key, call the `containsKey()` method. The `containsKey()` method takes one argument: the key.
5. To remove a key-value pair from the hash table, call the `remove()` method. The `remove()` method takes one argument: the key.

### Example

```java
HashTable<String, Integer> hashTable = new HashTable<>();

// Add some key-value pairs
hashTable.put("Mohamad", 1234567890);
hashTable.put("Samara", 9876543210);

// Get the value associated with a key
int phoneNumber = hashTable.get("Mohamad");

System.out.println(phoneNumber); // Output: 1234567890

// Check if the hash table contains a key
boolean containsKey = hashTable.containsKey("Samara");

System.out.println(containsKey); // Output: true

// Remove a key-value pair from the hash table
hashTable.remove("Samara");

// Check if the hash table contains the key that was removed
containsKey = hashTable.containsKey("Samara");

System.out.println(containsKey); // Output: false
```

### Walk-through

1. The first line of code creates a new hash table object.
2. The next two lines of code add some key-value pairs to the hash table.
3. The next line of code gets the value associated with the key "Mohamad".
4. The next line of code prints the value to the console.
5. The next line of code checks if the hash table contains the key "Samara".
6. The next line of code prints the result to the console.
7. The next line of code removes the key-value pair associated with the key "Samara".
8. The next line of code checks if the hash table still contains the key "Samara".
9. The next line of code prints the result to the console.

## Vocabulary/Definition List

| Term             | Definition                                                                                          |
|------------------|-----------------------------------------------------------------------------------------------------|
| Hash table       | A data structure that maps keys to values.                                                          |
| Key              | A unique identifier for a value in a hash table.                                                    |
| Value            | The data associated with a key in a hash table.                                                     |
| Bucket           | An array element in a hash table.                                                                   |
| Hash function    | A function that converts a key into a unique index in a hash table.                                 |
| Collision        | When two different keys hash to the same index in a hash table.                                     |
| Separate chaining | A method of handling collisions by storing a linked list of key-value pairs at each bucket.        |
| Open addressing  | A method of handling collisions by storing key-value pairs directly in the hash table array.        |

## Hash Table Cheat Sheet

* **Time complexity:**
    1. Insertion: O(1) on average, O(n) in the worst case
    2. Retrieval: O(1) on average, O(n) in the worst case
    3. Search: O(1) on average, O(n) in the worst case

* **Space complexity:** O(n)
* **Applications:**
    1. Caching
    2. Databases
    3. Compilers
    4. Networking

## Fill-in-the-Blank Worksheet**

1. A hash table is a data structure that maps ____ to ____.
2. A ____ is a unique identifier for a value in a hash table.
3. The ____ is the data associated with a key in a hash table.
4. A ____ is an array element in a hash table.
5. A ____ is a function that converts a key into a unique index in a hash table.
6. A ____ occurs when two different keys hash to the same index in a hash table.
7. ____ is a method of handling collisions by storing a linked list of key-value pairs at each bucket.
8. ____ is a method of handling collisions by storing key-value pairs directly in the hash table array.

## Answers

1. keys, values
2. key
3. value
4. bucket
5. hash function
6. collision
7. Separate chaining
8. Open addressing

## Map of the information:**

```java
Hash table
├── Key
├── Value
└── Bucket
    └── Collision
        ├── Separate chaining
        └── Open addressing
```

This map shows that a hash table is made up of buckets. Each bucket contains a collision handler. The collision handler is responsible for handling collisions, which occur when two different keys hash to the same index. There are two collision handlers: separate chaining and open addressing.

**Separate chaining** stores the key-value pairs in a linked list at each bucket. When a collision occurs, the new key-value pair is added to the linked list.

**Open addressing** stores the key-value pairs directly in the hash table array. When a collision occurs, a different index is found for the new key-value pair.

## Quiz

1. What is a hash table?
2. How does a hash function work?
3. What is a collision?
4. What is separate chaining?
5. What are some of the advantages and disadvantages of hash tables?

## Answers

1. A hash table is a data structure that maps keys to values.
2. A hash function takes any input and produces a unique output.
3. A collision occurs when two different keys have the same hash value.
4. Separate chaining is a collision resolution technique that uses linked lists to store key-value pairs that have the same hash value.
5. Advantages of hash tables include fast search and insertion times, and scalability. Disadvantages of hash tables include inefficiency in the presence of many collisions, and memory intensiveness.
