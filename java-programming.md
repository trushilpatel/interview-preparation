# Competitive Coding Preparation in Java

## Table of Contents- [Competitive Coding Preparation in Java](#competitive-coding-preparation-in-java)

- [Competitive Coding Preparation in Java](#competitive-coding-preparation-in-java)
  - [Table of Contents- Competitive Coding Preparation in Java](#table-of-contents--competitive-coding-preparation-in-java)
  - [1. Data Structures](#1-data-structures)
  - [2. Algorithms](#2-algorithms)
  - [3. Object-Oriented Programming (OOP)](#3-object-oriented-programming-oop)
  - [4. Java-Specific Concepts](#4-java-specific-concepts)
  - [5. Math and Number Theory](#5-math-and-number-theory)
  - [6. Input/Output Optimization](#6-inputoutput-optimization)
  - [7. Practice Platforms](#7-practice-platforms)
- [Different Ways to Take User Input in Java](#different-ways-to-take-user-input-in-java)
  - [1. Using `Scanner` Class](#1-using-scanner-class)
  - [2. Using `BufferedReader` Class](#2-using-bufferedreader-class)
  - [3. Using Command Line Arguments](#3-using-command-line-arguments)
- [Java Primitive Types - Range, Size, and Key Functions](#java-primitive-types---range-size-and-key-functions)
- [Java Boxed Types - Common Methods](#java-boxed-types---common-methods)
    - [Key Methods:](#key-methods)
- [Java String, StringBuilder, and StringBuffer - Common Methods](#java-string-stringbuilder-and-stringbuffer---common-methods)
      - [Key difference:](#key-difference)
  - [Common Methods of the String Class](#common-methods-of-the-string-class)
  - [Additional Notes:](#additional-notes)
  - [Common Methods of StringBuilder and StringBuffer](#common-methods-of-stringbuilder-and-stringbuffer)
  - [Key Differences:](#key-differences)
  - [Additional Notes:](#additional-notes-1)
- [Collections Framework design Diagram](#collections-framework-design-diagram)
  - [List Interface (e.g., ArrayList, LinkedList)](#list-interface-eg-arraylist-linkedlist)
  - [Set Interface (e.g., HashSet, TreeSet)](#set-interface-eg-hashset-treeset)
  - [Map Interface (e.g., HashMap, TreeMap)](#map-interface-eg-hashmap-treemap)
  - [Additional Notes:](#additional-notes-2)
  - [ArrayList](#arraylist)
  - [LinkedList](#linkedlist)
  - [HashSet](#hashset)
  - [TreeSet](#treeset)
  - [HashMap](#hashmap)
  - [TreeMap](#treemap)
  - [Stack](#stack)
  - [PriorityQueue](#priorityqueue)
  - [Trie](#trie)
  - [Additional Notes:](#additional-notes-3)
- [Comparison of Java Collections](#comparison-of-java-collections)
  - [Additional Notes:](#additional-notes-4)
- [Java Math Library Functions](#java-math-library-functions)
- [Java Arrays Class Functions](#java-arrays-class-functions)
- [Java Stream API Functions](#java-stream-api-functions)
  - [Stream Creation](#stream-creation)
  - [Intermediate Operations](#intermediate-operations)
  - [Terminal Operations](#terminal-operations)
- [Different Ways to Sort Collections in Java](#different-ways-to-sort-collections-in-java)
  - [1. Using `Collections.sort()` or `Comparable`](#1-using-collectionssort-or-comparable)
      - [Example:](#example)
    - [2. Using `Comparator`](#2-using-comparator)
    - [Example: Using `Comparator`](#example-using-comparator)
  - [3. Using Java 8 Streams](#3-using-java-8-streams)
      - [Example:](#example-1)
  - [4. Using Collections.reverseOrder()](#4-using-collectionsreverseorder)
      - [Example:](#example-2)
  - [5. Sorting with Lambdas](#5-sorting-with-lambdas)
      - [Example:](#example-3)
- [Summary of Sorting Approaches in Java](#summary-of-sorting-approaches-in-java)
  - [1. Using `Comparable`](#1-using-comparable)
  - [2. Using `Comparator`](#2-using-comparator-1)
  - [3. Using Java 8 Streams](#3-using-java-8-streams-1)
  - [4. Using `Collections.reverseOrder()`](#4-using-collectionsreverseorder-1)
  - [5. Sorting with Lambdas](#5-sorting-with-lambdas-1)

## 1. Data Structures

- **Arrays**: Manipulation, searching, sorting.
- **Strings**: String manipulation, palindrome, substring problems.
- **Linked Lists**: Singly, doubly, and circular lists, reversal, cycle detection.
- **Stacks and Queues**: Implementation, balanced parentheses, minimum/maximum operations.
- **Hashing**: HashMap, HashSet, handling collisions.
- **Trees**: Binary trees, Binary Search Trees (BST), AVL trees, DFS, BFS traversals.
- **Heaps**: Min-heap, max-heap, heapify, priority queues.
- **Graphs**: BFS, DFS, Dijkstra’s, Prim’s, Kruskal’s algorithms.
- **Trie**: Prefix tree, search, insertion, and deletion operations.

## 2. Algorithms

- **Sorting Algorithms**: QuickSort, MergeSort, HeapSort, BubbleSort.
- **Searching Algorithms**: Binary search, linear search, depth-first, breadth-first.
- **Recursion**: Backtracking problems, solving with recursion.
- **Dynamic Programming**: Knapsack, Longest Common Subsequence (LCS), Longest Increasing Subsequence (LIS), Matrix Chain Multiplication.
- **Greedy Algorithms**: Coin change, activity selection, Huffman coding.
- **Divide and Conquer**: Merge sort, quick sort, binary search tree.
- **Graph Algorithms**: Shortest path (Dijkstra’s, Bellman-Ford), Floyd Warshall, minimum spanning tree (Prim’s, Kruskal’s).
- **Bit Manipulation**: XOR, AND, OR, shifting bits for optimizations.

## 3. Object-Oriented Programming (OOP)

- **Encapsulation, Inheritance, Polymorphism, Abstraction**: Use cases, how to apply these concepts.
- **Design Patterns**: Singleton, Factory, Observer, Strategy patterns.

## 4. Java-Specific Concepts

- **Exception Handling**: `try-catch-finally`, checked vs unchecked exceptions.
- **Concurrency and Multithreading**: Creating threads, synchronization, thread-safe collections.
- **Collections Framework**: ArrayList, LinkedList, HashMap, TreeMap, HashSet, PriorityQueue.
- **Streams and Lambda Expressions**: Java 8 features for functional programming.

## 5. Math and Number Theory

- **Prime Numbers**: Sieve of Eratosthenes, primality tests.
- **Greatest Common Divisor (GCD)**: Euclidean algorithm.
- **Modular Arithmetic**: Modular exponentiation, modular inverses.
- **Combinatorics**: Permutations, combinations, Pascal’s triangle.
- **Number Theory**: LCM, prime factorization.

## 6. Input/Output Optimization

- **Fast Input/Output**: BufferedReader, PrintWriter, Scanner performance tricks.
- **Efficient String Handling**: StringBuilder vs String for concatenation.

## 7. Practice Platforms

- **LeetCode, Codeforces, HackerRank, CodeChef, GeeksforGeeks**: Platforms providing problems tailored for online assessments and coding challenges.

# Different Ways to Take User Input in Java

Java provides several ways to take user input. Below are some common methods:

## 1. Using `Scanner` Class

The `Scanner` class is one of the most common ways to read input from various sources like keyboard input, files, etc.

```java
import java.util.Scanner;

public class UserInputExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter your name: ");
        String name = scanner.nextLine();

        System.out.print("Enter your age: ");
        int age = scanner.nextInt();

        System.out.println("Name: " + name + ", Age: " + age);

        scanner.close();
    }
}
```

## 2. Using `BufferedReader` Class

`BufferedReader` can be used for more efficient reading of text from input streams.

```java
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;

public class UserInputExample {
    public static void main(String[] args) throws IOException {
        BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));

        System.out.print("Enter your name: ");
        String name = reader.readLine();

        System.out.print("Enter your age: ");
        int age = Integer.parseInt(reader.readLine());

        System.out.println("Name: " + name + ", Age: " + age);
    }
}

```

## 3. Using Command Line Arguments

You can also take inputs through command line arguments when running the program.

```java
public class UserInputExample {
    public static void main(String[] args) {
        if (args.length < 2) {
            System.out.println("Please provide name and age as command line arguments.");
            return;
        }

        String name = args[0];
        int age = Integer.parseInt(args[1]);

        System.out.println("Name: " + name + ", Age: " + age);
    }
}

```

# Java Primitive Types - Range, Size, and Key Functions

| **Type**  | **Min Value**              | **Max Value**             | **Range (10^n)**    | **Size (Bytes)**   | **Notes**                      |
| --------- | -------------------------- | ------------------------- | ------------------- | ------------------ | ------------------------------ |
| `Byte`    | -128                       | 127                       | ~10^2               | 1                  | Signed 8-bit integer           |
| `Short`   | -32,768                    | 32,767                    | ~10^4               | 2                  | Signed 16-bit integer          |
| `Integer` | -2,147,483,648             | 2,147,483,647             | ~10^9               | 4                  | Signed 32-bit integer          |
| `Long`    | -9,223,372,036,854,775,808 | 9,223,372,036,854,775,807 | ~10^18              | 8                  | Signed 64-bit integer          |
| `Float`   | 1.4E-45 (approx)           | 3.4E+38 (approx)          | ~10^-45 to 10^38    | 4                  | 32-bit IEEE 754 floating point |
| `Double`  | 4.9E-324 (approx)          | 1.8E+308 (approx)         | ~10^-324 to 10^308  | 8                  | 64-bit IEEE 754 floating point |
| `Boolean` | `false`                    | `true`                    | N/A                 | 1 (depends on JVM) | Represents true/false          |
| `Char`    | '\u0000' (0)               | '\uffff' (65,535)         | 0 to 2^16 (Unicode) | 2                  | Unsigned 16-bit character      |

# Java Boxed Types - Common Methods

| **Boxed Type** | **Common Methods**                                                                                                                                                       | **Description**                                                                                                                                 |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| `Byte`         | `Byte.parseByte(String s)`<br/>`Byte.valueOf(String s)`<br/>`byteValue()`                                                                                                | Parses a `String` into a `byte`.<br/>Converts a `String` to a `Byte` object.<br/>Returns the `byte` value of the `Byte` object.                 |
| `Short`        | `Short.parseShort(String s)`<br/>`Short.valueOf(String s)`<br/>`shortValue()`                                                                                            | Parses a `String` into a `short`.<br/>Converts a `String` to a `Short` object.<br/>Returns the `short` value of the `Short` object.             |
| `Integer`      | `Integer.parseInt(String s)`<br/>`Integer.valueOf(String s)`<br/>`intValue()`<br/>`compareTo(Integer anotherInt)`<br/>`Integer.toHexString(int i)`                       | Parses a `String` into an `int`.<br/>Converts a `String` to an `Integer` object.<br/>Compares this `Integer` with another.<br/>Converts to hex. |
| `Long`         | `Long.parseLong(String s)`<br/>`Long.valueOf(String s)`<br/>`longValue()`<br/>`compareTo(Long anotherLong)`<br/>`Long.toHexString(long l)`                               | Parses a `String` into a `long`.<br/>Converts a `String` to a `Long` object.<br/>Compares this `Long` with another.<br/>Converts to hex.        |
| `Float`        | `Float.parseFloat(String s)`<br/>`Float.valueOf(String s)`<br/>`floatValue()`<br/>`compareTo(Float anotherFloat)`<br/>`isNaN()`                                          | Parses a `String` into a `float`.<br/>Converts a `String` to a `Float` object.<br/>Checks if the value is `NaN` (Not a Number).                 |
| `Double`       | `Double.parseDouble(String s)`<br/>`Double.valueOf(String s)`<br/>`doubleValue()`<br/>`compareTo(Double anotherDouble)`<br/>`isNaN()`<br/>`Double.toHexString(double d)` | Parses a `String` into a `double`.<br/>Converts a `String` to a `Double` object.<br/>Compares `Double` values.<br/>Converts to hex.             |
| `Boolean`      | `Boolean.parseBoolean(String s)`<br/>`Boolean.valueOf(String s)`<br/>`booleanValue()`<br/>`compareTo(Boolean anotherBoolean)`                                            | Parses a `String` into a `boolean`.<br/>Converts a `String` to a `Boolean` object.<br/>Compares two `Boolean` objects.                          |
| `Character`    | `Character.isUpperCase(char ch)`<br/>`Character.isDigit(char ch)`<br/>`Character.toLowerCase(char ch)`<br/>`compareTo(Character anotherChar)`                            | Checks if a character is uppercase.<br/>Checks if a character is a digit.<br/>Converts character to lowercase.                                  |

### Key Methods:

1. **Parsing**: Each boxed type provides `parse<Type>()` methods to convert strings into corresponding primitives.
2. **Conversion**: Methods like `valueOf()` convert a string to an object of the boxed type.
3. **Value Retrieval**: Methods like `intValue()`, `longValue()`, etc., extract the primitive value from the boxed object.
4. **Comparison**: Methods like `compareTo()` compare two objects of the same type.
5. **Utility**: Additional methods like `toHexString()`, `isNaN()`, `isUpperCase()`, and `isDigit()` provide useful utility functions.

# Java String, StringBuilder, and StringBuffer - Common Methods

#### Key difference:

1. **Immutability**: `String` is immutable, meaning once created, it cannot be changed. `StringBuilder` and `StringBuffer` are mutable.
2. **Thread Safety**: `StringBuffer` is synchronized and thread-safe, while `StringBuilder` is not.
3. **Performance**: `StringBuilder` is faster than `StringBuffer` as it does not have the overhead of synchronization.

## Common Methods of the String Class

| **Method**                                     | **Description**                                                                                              |
| ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| `charAt(int index)`                            | Returns the character at the specified index.                                                                |
| `compareTo(String anotherString)`              | Compares two strings lexicographically.                                                                      |
| `compareToIgnoreCase(String str)`              | Compares two strings lexicographically, ignoring case differences.                                           |
| `concat(String str)`                           | Concatenates the specified string to the end of this string.                                                 |
| `contains(CharSequence sequence)`              | Returns `true` if this string contains the specified sequence of char values.                                |
| `endsWith(String suffix)`                      | Returns `true` if this string ends with the specified suffix.                                                |
| `equals(Object anObject)`                      | Compares this string to the specified object for equality.                                                   |
| `equalsIgnoreCase(String anotherString)`       | Compares this string to another string, ignoring case considerations.                                        |
| `format(String format, Object... args)`        | Returns a formatted string using the specified format string and arguments.                                  |
| `indexOf(int ch)`                              | Returns the index of the first occurrence of the specified character.                                        |
| `indexOf(String str)`                          | Returns the index of the first occurrence of the specified substring.                                        |
| `isEmpty()`                                    | Returns `true` if this string is empty (length is 0).                                                        |
| `lastIndexOf(int ch)`                          | Returns the index of the last occurrence of the specified character.                                         |
| `lastIndexOf(String str)`                      | Returns the index of the last occurrence of the specified substring.                                         |
| `length()`                                     | Returns the length of this string.                                                                           |
| `replace(char oldChar, char newChar)`          | Returns a new string resulting from replacing all occurrences of `oldChar` with `newChar`.                   |
| `replaceAll(String regex, String replacement)` | Replaces each substring of this string that matches the given regular expression with the given replacement. |
| `split(String regex)`                          | Splits this string around matches of the given regular expression.                                           |
| `startsWith(String prefix)`                    | Returns `true` if this string starts with the specified prefix.                                              |
| `substring(int beginIndex)`                    | Returns a new string that is a substring of this string.                                                     |
| `substring(int beginIndex, int endIndex)`      | Returns a new string that is a substring of this string, starting from `beginIndex` to `endIndex`.           |
| `toLowerCase()`                                | Converts all of the characters in this string to lower case.                                                 |
| `toUpperCase()`                                | Converts all of the characters in this string to upper case.                                                 |
| `trim()`                                       | Returns a copy of the string, with leading and trailing whitespace omitted.                                  |
| `valueOf(Object obj)`                          | Returns the string representation of the specified object.                                                   |

## Additional Notes:

- **Immutable**: Strings in Java are immutable, meaning once created, their values cannot be changed.
- **Performance**: For heavy manipulations, consider using `StringBuilder` or `StringBuffer`.

## Common Methods of StringBuilder and StringBuffer

| **Method**                                | **Description**                                                       |
| ----------------------------------------- | --------------------------------------------------------------------- |
| `append(String str)`                      | Appends the specified string to the end of this string builder.       |
| `insert(int offset, String str)`          | Inserts the specified string at the specified position.               |
| `delete(int start, int end)`              | Removes the characters in a substring from this sequence.             |
| `deleteCharAt(int index)`                 | Removes the character at the specified position.                      |
| `replace(int start, int end, String str)` | Replaces the substring with the specified string.                     |
| `reverse()`                               | Reverses the characters in this string builder.                       |
| `capacity()`                              | Returns the current capacity of the string builder.                   |
| `length()`                                | Returns the number of characters in the string builder.               |
| `toString()`                              | Converts this string builder to a string.                             |
| `charAt(int index)`                       | Returns the character at the specified index.                         |
| `indexOf(String str)`                     | Returns the index of the first occurrence of the specified substring. |
| `lastIndexOf(String str)`                 | Returns the index of the last occurrence of the specified substring.  |
| `setCharAt(int index, char ch)`           | Sets the character at the specified index to the specified character. |

## Key Differences:

1. **Immutability**: Both `StringBuilder` and `StringBuffer` are mutable, meaning their values can be changed after creation.
2. **Thread Safety**: `StringBuffer` is synchronized and thread-safe, while `StringBuilder` is not.
3. **Performance**: `StringBuilder` is generally faster than `StringBuffer` because it does not have the overhead of synchronization.

## Additional Notes:

- Use `StringBuilder` for single-threaded scenarios for better performance.
- Use `StringBuffer` in multi-threaded scenarios where thread safety is required.

# Collections Framework design Diagram

```plaintext

                           +-----------------------------+
                           |          Iterable            |
                           +-----------------------------+
                           | +iterator()                 |
                           +-----------------------------+
                                     |
                           +-----------------------------+
                           |         Collection           |
                           +-----------------------------+
                           | +add(E e)                   |
                           | +remove(Object o)           |
                           | +contains(Object o)         |
                           | +size()                     |
                           | +isEmpty()                  |
                           | +clear()                    |
                           +-----------------------------+
                                     |
        +-----------------+----------+--------------+------------+
        |                 |                         |            |
   +-----------+     +------------+         +------------+    +------------+
   |   List    |     |    Set     |         |   Queue    |    |   Deque     |
   +-----------+     +------------+         +------------+    +------------+
   | +get(int index) | +add(E e)  |         | +offer(E e)|    | +addFirst(E e) |
   | +add(E e)       | +remove()  |         | +poll()    |    | +addLast(E e)  |
   | +remove(int)    | +contains()|         | +peek()    |    | +removeFirst() |
   | +size()         | +size()    |         | +remove()  |    | +removeLast()  |
   +-----------+     +------------+         +------------+    +------------+
        |                 |                         |            |
   +-----------+     +------------+            +------------+    |
   | Abstract  |     | Abstract   |            | Abstract   |    |
   |   List    |     |    Set     |            |    Queue   |    |
   +-----------+     +------------+            +------------+    |
        |                 |                         |            |
        |                 |                         |            |
   +------------+      +------------+       +------------+   +--------------+
   |  ArrayList |      |   HashSet   |      | LinkedList  |   | ArrayDeque   |
   +------------+      +------------+       +------------+   +--------------+
   | +add(E e)  |      | +add(E e)  |       | +add(E e)   |   | +add(E e)    |
   | +get(int)  |      | +contains()|       | +poll()     |   | +poll()      |
   | +remove()  |      | +remove()  |       | +remove()   |   | +peek()      |
   +------------+      +------------+       +------------+   +--------------+
                                                    |
                                                    +-----------------------+
                                                    | PriorityBlockingQueue |
                                                    +-----------------------+
                                                    | +offer(E e)            |
                                                    | +poll()                |
                                                    | +remove()              |
                                                    +-----------------------+

    +--------------------+             +-----------------------+
    |       Vector        |             |      Stack            |
    +--------------------+             +-----------------------+
    | +add(E e)           |             | +push(E e)            |
    | +get(int index)     |             | +pop()                |
    | +remove(int index)  |             | +peek()               |
    +--------------------+             +-----------------------+

    +------------------------------------------------+
    |                Map Interface                   |
    +------------------------------------------------+
    | +put(K key, V value)                           |
    | +get(Object key)                               |
    | +remove(Object key)                            |
    | +containsKey(Object key)                       |
    | +size()                                        |
    +------------------------------------------------+
                     |
   +--------------------------+           +--------------------------+
   |         HashMap           |           |       TreeMap            |
   +--------------------------+           +--------------------------+
   | +put(K key, V value)      |           | +put(K key, V value)     |
   | +get(Object key)          |           | +get(Object key)         |
   | +containsKey(Object key)  |           | +containsKey(Object key) |
   | +remove(Object key)       |           | +remove(Object key)      |
   +--------------------------+           +--------------------------+
             |
             +------------------------------+
             | ConcurrentHashMap             |
             +------------------------------+
             | +put(K key, V value)          |
             | +get(Object key)              |
             | +containsKey(Object key)      |
             +------------------------------+

    +------------------------+       +--------------------------+
    |        SortedMap        |       |       TreeSet            |
    +------------------------+       +--------------------------+
    | +firstKey()             |       | +add(E e)                |
    | +lastKey()              |       | +contains(Object o)      |
    | +subMap(K fromKey, K toKey)|    | +remove(Object o)        |
    +------------------------+       +--------------------------+

    +--------------------------------------------------+
    |                    Arrays Class                  |
    +--------------------------------------------------+
    | +sort(Object[] a)                                |
    | +binarySearch(Object[] a, Object key)            |
    | +asList(T... a)                                  |
    +--------------------------------------------------+

    +--------------------------------------------------+
    |                ArrayBlockingQueue                |
    +--------------------------------------------------+
    | +put(E e)                                        |
    | +take()                                          |
    | +poll()                                          |
    | +remove()                                        |
    +--------------------------------------------------+
```

## List Interface (e.g., ArrayList, LinkedList)

| **Method**                  | **Description**                                                                                                                   |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| `add(E e)`                  | Appends the specified element to the end of the list.                                                                             |
| `add(int index, E element)` | Inserts the specified element at the specified position in the list.                                                              |
| `remove(int index)`         | Removes the element at the specified position in the list.                                                                        |
| `remove(Object o)`          | Removes the first occurrence of the specified element from this list, if it is present.                                           |
| `get(int index)`            | Returns the element at the specified position in this list.                                                                       |
| `set(int index, E element)` | Replaces the element at the specified position in this list with the specified element.                                           |
| `size()`                    | Returns the number of elements in the list.                                                                                       |
| `contains(Object o)`        | Returns `true` if this list contains the specified element.                                                                       |
| `indexOf(Object o)`         | Returns the index of the first occurrence of the specified element in this list, or -1 if this list does not contain the element. |
| `clear()`                   | Removes all of the elements from this list.                                                                                       |

## Set Interface (e.g., HashSet, TreeSet)

| **Method**           | **Description**                                                      |
| -------------------- | -------------------------------------------------------------------- |
| `add(E e)`           | Adds the specified element to this set if it is not already present. |
| `remove(Object o)`   | Removes the specified element from this set if it is present.        |
| `contains(Object o)` | Returns `true` if this set contains the specified element.           |
| `size()`             | Returns the number of elements in this set.                          |
| `clear()`            | Removes all of the elements from this set.                           |
| `isEmpty()`          | Returns `true` if this set contains no elements.                     |

## Map Interface (e.g., HashMap, TreeMap)

| **Method**                    | **Description**                                                                                                |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `put(K key, V value)`         | Associates the specified value with the specified key in this map.                                             |
| `get(Object key)`             | Returns the value to which the specified key is mapped, or `null` if this map contains no mapping for the key. |
| `remove(Object key)`          | Removes the mapping for the specified key from this map if present.                                            |
| `containsKey(Object key)`     | Returns `true` if this map contains a mapping for the specified key.                                           |
| `containsValue(Object value)` | Returns `true` if this map maps one or more keys to the specified value.                                       |
| `size()`                      | Returns the number of key-value mappings in this map.                                                          |
| `keySet()`                    | Returns a `Set` view of the keys contained in this map.                                                        |
| `values()`                    | Returns a `Collection` view of the values contained in this map.                                               |
| `entrySet()`                  | Returns a `Set` view of the mappings contained in this map.                                                    |

## Additional Notes:

- **Performance**: Different collection types have different performance characteristics. For example, `ArrayList` is faster for indexed access, while `LinkedList` is faster for insertion and deletion.
- **Thread Safety**: Use `Collections.synchronizedList`, `Collections.synchronizedSet`, and `Collections.synchronizedMap` to make collections thread-safe.

## ArrayList

| **Method**                  | **Description**                                                                         |
| --------------------------- | --------------------------------------------------------------------------------------- |
| `add(E e)`                  | Appends the specified element to the end of the list.                                   |
| `add(int index, E element)` | Inserts the specified element at the specified position in the list.                    |
| `remove(int index)`         | Removes the element at the specified position in the list.                              |
| `get(int index)`            | Returns the element at the specified position in this list.                             |
| `set(int index, E element)` | Replaces the element at the specified position in this list with the specified element. |
| `clear()`                   | Removes all of the elements from this list.                                             |
| `size()`                    | Returns the number of elements in the list.                                             |

## LinkedList

| **Method**       | **Description**                                              |
| ---------------- | ------------------------------------------------------------ |
| `add(E e)`       | Appends the specified element to the end of the list.        |
| `addFirst(E e)`  | Inserts the specified element at the beginning of this list. |
| `addLast(E e)`   | Appends the specified element to the end of this list.       |
| `removeFirst()`  | Removes and returns the first element of this list.          |
| `removeLast()`   | Removes and returns the last element of this list.           |
| `get(int index)` | Returns the element at the specified position in this list.  |
| `size()`         | Returns the number of elements in the list.                  |

## HashSet

| **Method**           | **Description**                                                      |
| -------------------- | -------------------------------------------------------------------- |
| `add(E e)`           | Adds the specified element to this set if it is not already present. |
| `remove(Object o)`   | Removes the specified element from this set if it is present.        |
| `contains(Object o)` | Returns `true` if this set contains the specified element.           |
| `size()`             | Returns the number of elements in this set.                          |
| `isEmpty()`          | Returns `true` if this set contains no elements.                     |
| `clear()`            | Removes all of the elements from this set.                           |

## TreeSet

| **Method**    | **Description**                                                                                                              |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| `add(E e)`    | Adds the specified element to this set.                                                                                      |
| `first()`     | Returns the first (lowest) element currently in this set.                                                                    |
| `last()`      | Returns the last (highest) element currently in this set.                                                                    |
| `higher(E e)` | Returns the least element in this set greater than the specified element, or `null` if there is no such element.             |
| `floor(E e)`  | Returns the greatest element in this set less than or equal to the specified element, or `null` if there is no such element. |
| `size()`      | Returns the number of elements in this set.                                                                                  |

## HashMap

| **Method**                    | **Description**                                                                                                |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `put(K key, V value)`         | Associates the specified value with the specified key in this map.                                             |
| `get(Object key)`             | Returns the value to which the specified key is mapped, or `null` if this map contains no mapping for the key. |
| `remove(Object key)`          | Removes the mapping for the specified key from this map if present.                                            |
| `containsKey(Object key)`     | Returns `true` if this map contains a mapping for the specified key.                                           |
| `containsValue(Object value)` | Returns `true` if this map maps one or more keys to the specified value.                                       |
| `keySet()`                    | Returns a `Set` view of the keys contained in this map.                                                        |
| `values()`                    | Returns a `Collection` view of the values contained in this map.                                               |

## TreeMap

| **Method**            | **Description**                                                                                      |
| --------------------- | ---------------------------------------------------------------------------------------------------- |
| `put(K key, V value)` | Associates the specified value with the specified key in this map.                                   |
| `firstKey()`          | Returns the first (lowest) key currently in this map.                                                |
| `lastKey()`           | Returns the last (highest) key currently in this map.                                                |
| `higherKey(K key)`    | Returns the least key greater than the specified key, or `null` if there is no such key.             |
| `floorKey(K key)`     | Returns the greatest key less than or equal to the specified key, or `null` if there is no such key. |
| `size()`              | Returns the number of key-value mappings in this map.                                                |

## Stack

| **Method**         | **Description**                                                                                    |
| ------------------ | -------------------------------------------------------------------------------------------------- |
| `push(E item)`     | Pushes an item onto the top of this stack.                                                         |
| `pop()`            | Removes the object at the top of this stack and returns that object as the value of this function. |
| `peek()`           | Looks at the object at the top of this stack without removing it from the stack.                   |
| `isEmpty()`        | Tests if this stack is empty.                                                                      |
| `search(Object o)` | Returns the 1-based position where an object is on this stack.                                     |

## PriorityQueue

| **Method** | **Description**                                                                                   |
| ---------- | ------------------------------------------------------------------------------------------------- |
| `add(E e)` | Inserts the specified element into this priority queue.                                           |
| `poll()`   | Retrieves and removes the head of this queue, or returns `null` if this queue is empty.           |
| `peek()`   | Retrieves, but does not remove, the head of this queue, or returns `null` if this queue is empty. |
| `size()`   | Returns the number of elements in this queue.                                                     |

## Trie

A Trie (or prefix tree) is a special type of tree used to store associative data structures. Below is a list of commonly used functions associated with Trie operations:

| Function Name                           | Description                                                                                                                        |
| --------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| `insert(String word)`                   | Inserts a word into the Trie, creating nodes for each character in the word if they don't already exist.                           |
| `search(String word)`                   | Searches for a word in the Trie. Returns `true` if the word exists, otherwise returns `false`.                                     |
| `startsWith(String prefix)`             | Checks if there is any word in the Trie that starts with the given prefix. Returns `true` if it exists, otherwise returns `false`. |
| `delete(String word)`                   | Removes a word from the Trie. If the word does not exist, the function may do nothing or return an indication of failure.          |
| `getWordsWithPrefix(String prefix)`     | Retrieves all words in the Trie that start with the given prefix. Returns a list of words.                                         |
| `countWordsEqualTo(String word)`        | Counts how many times the exact word appears in the Trie. Returns an integer count.                                                |
| `countWordsStartingWith(String prefix)` | Counts how many words in the Trie start with the given prefix. Returns an integer count.                                           |
| `isEmpty()`                             | Checks if the Trie is empty (contains no words). Returns `true` if empty, otherwise `false`.                                       |
| `getSize()`                             | Returns the number of words currently stored in the Trie.                                                                          |

## Additional Notes:

- **Performance**: Each collection type has different performance characteristics based on their implementation. Choose the one that suits your needs based on time complexity and functionality.
- **Thread Safety**: For thread-safe versions of collections, consider using `Collections.synchronizedList`, `Collections.synchronizedSet`, and `Collections.synchronizedMap`.

# Comparison of Java Collections

| **Collection Type** | **Add (Write)** | **Get (Read)** | **Remove (Delete)** | **Contains** | **Iteration** | **Memory Usage** | **Notes**                                                          |
| ------------------- | --------------- | -------------- | ------------------- | ------------ | ------------- | ---------------- | ------------------------------------------------------------------ |
| **ArrayList**       | O(1)            | O(1)           | O(n)                | O(n)         | O(n)          | Low              | Fast for random access; resizing can be costly.                    |
| **LinkedList**      | O(1)            | O(n)           | O(n)                | O(n)         | O(n)          | Moderate         | Fast insertions/deletions; slower for access.                      |
| **HashSet**         | O(1)            | O(1)           | O(1)                | O(1)         | O(n)          | Low              | Unordered; no duplicates; fast operations.                         |
| **TreeSet**         | O(log n)        | O(log n)       | O(log n)            | O(log n)     | O(n)          | Moderate         | Sorted; slower than HashSet; allows range queries.                 |
| **HashMap**         | O(1)            | O(1)           | O(1)                | O(1)         | O(n)          | Moderate         | Unordered key-value pairs; fast operations.                        |
| **TreeMap**         | O(log n)        | O(log n)       | O(log n)            | O(log n)     | O(n)          | Moderate         | Sorted; slower than HashMap; allows range queries.                 |
| **Stack**           | O(1)            | O(1)           | O(1)                | O(n)         | O(n)          | Low              | LIFO structure; primarily for backtracking.                        |
| **PriorityQueue**   | O(log n)        | O(1)           | O(log n)            | O(n)         | O(n)          | Moderate         | Orders elements; faster for accessing the highest/lowest priority. |

## Additional Notes:

- **Write (Add)**: Refers to the time complexity for adding an element to the collection.
- **Read (Get)**: Refers to the time complexity for retrieving an element from the collection.
- **Delete (Remove)**: Refers to the time complexity for removing an element from the collection.
- **Contains**: Refers to the time complexity for checking if an element exists in the collection.
- **Iteration**: Refers to the time complexity for iterating through all elements in the collection.
- **Memory Usage**: General estimate of how memory-intensive the collection is.

# Java Math Library Functions

The Java `Math` class provides a variety of mathematical functions. Below is a list of commonly used functions:

| Function Name               | Description                                                                                                    |
| --------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `abs(int a)`                | Returns the absolute value of an integer.                                                                      |
| `abs(double a)`             | Returns the absolute value of a double.                                                                        |
| `sqrt(double a)`            | Returns the square root of a double value.                                                                     |
| `pow(double a, double b)`   | Returns the value of the first argument raised to the power of the second argument.                            |
| `max(int a, int b)`         | Returns the greater of two integers.                                                                           |
| `max(double a, double b)`   | Returns the greater of two double values.                                                                      |
| `min(int a, int b)`         | Returns the smaller of two integers.                                                                           |
| `min(double a, double b)`   | Returns the smaller of two double values.                                                                      |
| `round(double a)`           | Rounds a double to the nearest integer.                                                                        |
| `floor(double a)`           | Returns the largest integer less than or equal to the argument.                                                |
| `ceil(double a)`            | Returns the smallest integer greater than or equal to the argument.                                            |
| `random()`                  | Returns a double value with a positive sign, greater than or equal to 0.0 and less than 1.0.                   |
| `sin(double a)`             | Returns the sine of the specified angle (in radians).                                                          |
| `cos(double a)`             | Returns the cosine of the specified angle (in radians).                                                        |
| `tan(double a)`             | Returns the tangent of the specified angle (in radians).                                                       |
| `asin(double a)`            | Returns the arcsine of a value, in radians.                                                                    |
| `acos(double a)`            | Returns the arccosine of a value, in radians.                                                                  |
| `atan(double a)`            | Returns the arctangent of a value, in radians.                                                                 |
| `atan2(double y, double x)` | Returns the angle theta from the conversion of rectangular coordinates (x, y) to polar coordinates (r, theta). |
| `log(double a)`             | Returns the natural logarithm (base e) of a double value.                                                      |
| `log10(double a)`           | Returns the base 10 logarithm of a double value.                                                               |
| `exp(double a)`             | Returns Euler's number raised to the power of a double value.                                                  |
| `hypot(double x, double y)` | Returns the hypotenuse of a right triangle given its two legs.                                                 |

# Java Arrays Class Functions

The Java `Arrays` class provides various utility functions for manipulating arrays. Below is a list of commonly used functions:

| Function Name                                   | Description                                                                                                       |
| ----------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `copyOf(int[] original, int newLength)`         | Copies the specified array, truncating or padding with zeros (if necessary) so the copy has the specified length. |
| `copyOfRange(int[] original, int from, int to)` | Copies the specified range of the specified array into a new array.                                               |
| `sort(int[] a)`                                 | Sorts the specified array into ascending order.                                                                   |
| `sort(int[] a, int fromIndex, int toIndex)`     | Sorts the specified range of the array into ascending order.                                                      |
| `binarySearch(int[] a, int key)`                | Searches the specified array for the specified value using the binary search algorithm.                           |
| `fill(int[] a, int val)`                        | Assigns the specified value to each element of the specified array.                                               |
| `equals(int[] a, int[] a2)`                     | Returns `true` if the two specified arrays are equal to one another.                                              |
| `toString(int[] a)`                             | Returns a string representation of the contents of the specified array.                                           |
| `asList(T... a)`                                | Returns a fixed-size list backed by the specified array.                                                          |
| `stream(int[] array)`                           | Returns a sequential `Stream` with the specified array as its source.                                             |

# Java Stream API Functions

The Java Stream API provides various methods for processing sequences of elements (such as collections). Below is a list of commonly used functions:

## Stream Creation

| Function Name                                | Description                                                                                                                                                  |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `Stream.of(T... values)`                     | Creates a stream from the specified values.                                                                                                                  |
| `Arrays.stream(T[] array)`                   | Creates a stream from the specified array.                                                                                                                   |
| `Collection.stream()`                        | Returns a sequential stream with the collection as its source.                                                                                               |
| `Stream.generate(Supplier<T> s)`             | Creates an infinite sequential ordered stream where each element is generated by the provided `Supplier`.                                                    |
| `Stream.iterate(T seed, UnaryOperator<T> f)` | Creates an infinite sequential ordered stream where the first element is `seed`, and each subsequent element is generated by applying the provided function. |

## Intermediate Operations

| Function Name                                                        | Description                                                                                                                                                                  |
| -------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `filter(Predicate<? super T> predicate)`                             | Returns a stream consisting of the elements that match the given predicate.                                                                                                  |
| `map(Function<? super T, ? extends R> mapper)`                       | Returns a stream consisting of the results of applying the given function to the elements of this stream.                                                                    |
| `flatMap(Function<? super T, ? extends Stream<? extends R>> mapper)` | Returns a stream consisting of the results of replacing each element of this stream with the contents of a mapped stream produced by applying the provided mapping function. |
| `distinct()`                                                         | Returns a stream consisting of the distinct elements (according to `Object.equals()`) of this stream.                                                                        |
| `sorted()`                                                           | Returns a stream consisting of the elements sorted in natural order.                                                                                                         |
| `sorted(Comparator<? super T> comparator)`                           | Returns a stream consisting of the elements sorted according to the provided comparator.                                                                                     |
| `limit(long maxSize)`                                                | Returns a stream consisting of the elements of this stream, truncated to be no longer than the specified size.                                                               |
| `skip(long n)`                                                       | Returns a stream consisting of the remaining elements after discarding the first `n` elements of this stream.                                                                |

## Terminal Operations

| Function Name                                       | Description                                                                                                                     |
| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| `forEach(Consumer<? super T> action)`               | Performs an action for each element of the stream.                                                                              |
| `collect(Collector<? super T, A, R> collector)`     | Performs a mutable reduction operation on the elements of the stream using a `Collector`.                                       |
| `reduce(T identity, BinaryOperator<T> accumulator)` | Performs a reduction on the elements of the stream using an associative accumulation function and returns an `Optional`.        |
| `count()`                                           | Returns the count of elements in the stream.                                                                                    |
| `findFirst()`                                       | Returns an `Optional` describing the first element of the stream, or an empty `Optional` if the stream is empty.                |
| `findAny()`                                         | Returns an `Optional` describing some element of the stream, or an empty `Optional` if the stream is empty.                     |
| `anyMatch(Predicate<? super T> predicate)`          | Returns whether any elements of this stream match the given predicate.                                                          |
| `allMatch(Predicate<? super T> predicate)`          | Returns whether all elements of this stream match the given predicate.                                                          |
| `noneMatch(Predicate<? super T> predicate)`         | Returns whether no elements of this stream match the given predicate.                                                           |
| `toArray()`                                         | Returns an array containing the elements of this stream.                                                                        |
| `toArray(IntFunction<A[]> generator)`               | Returns an array containing the elements of this stream; the runtime type of the returned array is that of the specified array. |

# Different Ways to Sort Collections in Java

Java provides multiple ways to sort collections. Here are some common methods:

## 1. Using `Collections.sort()` or `Comparable`

You can use the `Collections.sort()` method to sort a list of objects that implement the `Comparable` interface.

#### Example:

```java
import java.util.ArrayList;
import java.util.Collections;
import java.util.List;

class Fruit implements Comparable<Fruit> {
    String name;
    int weight;

    Fruit(String name, int weight) {
        this.name = name;
        this.weight = weight;
    }

    @Override
    public int compareTo(Fruit other) {
        return this.weight - other.weight; // Sort by weight
    }

    @Override
    public String toString() {
        return name + " (" + weight + ")";
    }
}

public class SortExample {
    public static void main(String[] args) {
        List<Fruit> fruits = new ArrayList<>();
        fruits.add(new Fruit("Apple", 150));
        fruits.add(new Fruit("Banana", 120));
        fruits.add(new Fruit("Orange", 130));

        Collections.sort(fruits);
        System.out.println("Sorted by weight: " + fruits);
    }
}
```

### 2. Using `Comparator`

The `Comparator` interface allows for defining multiple different orderings. You implement the `compare()` method.

### Example: Using `Comparator`

```java
import java.util.ArrayList;
import java.util.Collections;
import java.util.Comparator;
import java.util.List;

class Person {
    String name;
    int age;

    Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    @Override
    public String toString() {
        return "Person{name='" + name + "', age=" + age + "}";
    }
}

public class ComparatorExample {
    public static void main(String[] args) {
        List<Person> people = new ArrayList<>();
        people.add(new Person("Alice", 30));
        people.add(new Person("Bob", 25));
        people.add(new Person("Charlie", 35));

        // Sort by age using Comparator
        Collections.sort(people, Comparator.comparingInt(person -> person.age));
        System.out.println("Sorted by age using Comparator: " + people);

        // Sort by name using Comparator
        Collections.sort(people, Comparator.comparing(person -> person.name));
        System.out.println("Sorted by name using Comparator: " + people);
    }
}
```

## 3. Using Java 8 Streams

Java 8 introduced streams, which provide a modern way to sort collections.

#### Example:

```java
import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;

public class StreamSortExample {
    public static void main(String[] args) {
        List<String> names = Arrays.asList("Charlie", "Alice", "Bob");

        List<String> sortedNames = names.stream()
                .sorted()
                .collect(Collectors.toList());

        System.out.println("Sorted names: " + sortedNames);
    }
}

```

## 4. Using Collections.reverseOrder()

You can sort a collection in reverse order using `Collections.reverseOrder()`.

#### Example:

```java
import java.util.ArrayList;
import java.util.Collections;
import java.util.List;

public class ReverseSortExample {
    public static void main(String[] args) {
        List<Integer> numbers = new ArrayList<>();
        numbers.add(5);
        numbers.add(3);
        numbers.add(8);

        Collections.sort(numbers, Collections.reverseOrder());
        System.out.println("Sorted in reverse order: " + numbers);
    }
}
```

## 5. Sorting with Lambdas

In Java 8 and above, you can use lambda expressions to define the sorting criteria inline.

#### Example:

```java
import java.util.ArrayList;
import java.util.Collections;
import java.util.List;

public class LambdaSortExample {
    public static void main(String[] args) {
        List<String> fruits = new ArrayList<>();
        fruits.add("Banana");
        fruits.add("Apple");
        fruits.add("Orange");

        // Sort using lambda
        Collections.sort(fruits, (a, b) -> b.compareTo(a)); // Sort in reverse order
        System.out.println("Sorted fruits in reverse order: " + fruits);
    }
}
```

# Summary of Sorting Approaches in Java

Java provides various methods for sorting collections, catering to different requirements. Here's a summary of the key approaches:

## 1. Using `Comparable`

- **Description**: Implemented by the class whose objects need to be sorted.
- **Method**: Defines a single natural ordering through the `compareTo()` method.
- **Use Case**: Simple and natural sorting based on a single field.

## 2. Using `Comparator`

- **Description**: Allows custom sorting logic to be defined in a separate class or as an anonymous class/lambda.
- **Method**: Uses the `compare()` method to allow multiple sorting criteria.
- **Use Case**: Useful when you need different ways of sorting the same object type.

## 3. Using Java 8 Streams

- **Description**: Provides a modern approach to sort collections using functional programming concepts.
- **Method**: Utilizes the `sorted()` method on streams to sort collections.
- **Use Case**: Suitable for chaining operations and working with large datasets in a concise manner.

## 4. Using `Collections.reverseOrder()`

- **Description**: A built-in utility for sorting in reverse order.
- **Method**: Uses `Collections.sort()` with `Collections.reverseOrder()` for descending sort.
- **Use Case**: When you need a simple way to sort collections in descending order.

## 5. Sorting with Lambdas

- **Description**: Allows inline definition of sorting criteria using lambda expressions.
- **Method**: Uses the `sort()` method with a lambda function for custom sorting.
- **Use Case**: Convenient for short and specific sorting logic without needing a separate `Comparator` class.

These methods cover a range of sorting needs, from simple natural ordering to complex custom criteria, making Java collections versatile and easy to manage.
