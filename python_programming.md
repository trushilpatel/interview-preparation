
# Competitive Coding Preparation in Python

## Table of Contents - [Competitive Coding Preparation in Python](#competitive-coding-preparation-in-python)

- [Competitive Coding Preparation in Python](#competitive-coding-preparation-in-python)
  - [Table of Contents - Competitive Coding Preparation in Python](#table-of-contents--competitive-coding-preparation-in-python)
  - [1. Data Structures](#1-data-structures)
  - [2. Algorithms](#2-algorithms)
  - [3. Object-Oriented Programming (OOP)](#3-object-oriented-programming-oop)
  - [4. Python-Specific Concepts](#4-python-specific-concepts)
  - [5. Math and Number Theory](#5-math-and-number-theory)
  - [6. Input/Output Optimization](#6-inputoutput-optimization)
  - [7. Practice Platforms](#7-practice-platforms)
- [Different Ways to Take User Input in Python](#different-ways-to-take-user-input-in-python)
  - [1. Using `input()` Function](#1-using-input-function)
  - [2. Using `sys.stdin` for Faster Input](#2-using-sysstdin-for-faster-input)
  - [3. Using Command Line Arguments](#3-using-command-line-arguments)
- [Python Primitive Types - Range, Size, and Key Functions](#python-primitive-types---range-size-and-key-functions)
- [Python Mutable vs Immutable Types](#python-mutable-vs-immutable-types)
  - [Key Mutable Types](#key-mutable-types)
  - [Key Immutable Types](#key-immutable-types)
- [Python Strings - Common Methods](#python-strings---common-methods)
  - [Additional Notes:](#additional-notes)
- [Collections Framework in Python](#collections-framework-in-python)
  - [List](#list)
  - [Set](#set)
  - [Dictionary](#dictionary)
  - [Tuple](#tuple)
  - [Deque](#deque)
  - [Heap (using `heapq`)](#heap-using-heapq)
  - [Priority Queue](#priority-queue)
  - [Trie (using dictionary)](#trie-using-dictionary)
  - [Additional Notes:](#additional-notes-1)
- [Comparison of Python Collections](#comparison-of-python-collections)
  - [Additional Notes:](#additional-notes-2)
- [Python Math Library Functions](#python-math-library-functions)
- [Python Arrays (using `array` module)](#python-arrays-using-array-module)
- [Python List Comprehension and Generator Expressions](#python-list-comprehension-and-generator-expressions)
  - [List Comprehension](#list-comprehension)
  - [Generator Expressions](#generator-expressions)
- [Different Ways to Sort Collections in Python](#different-ways-to-sort-collections-in-python)
  - [1. Using `sort()` Method](#1-using-sort-method)
      - [Example:](#example)
  - [2. Using `sorted()` Function](#2-using-sorted-function)
      - [Example:](#example-1)
  - [3. Sorting with Lambda Functions](#3-sorting-with-lambda-functions)
      - [Example:](#example-2)
- [Summary of Sorting Approaches in Python](#summary-of-sorting-approaches-in-python)
  - [1. Using `sort()` Method](#1-using-sort-method-1)
  - [2. Using `sorted()` Function](#2-using-sorted-function-1)
  - [3. Sorting with Lambda Functions](#3-sorting-with-lambda-functions-1)

---

## 1. Data Structures

- **Arrays (Lists)**: List operations, slicing, sorting, searching.
- **Strings**: String manipulations, substrings, palindrome problems.
- **Linked Lists**: Implementation using classes, reversal, cycle detection.
- **Stacks and Queues**: Stack using `list`, queue using `deque` from `collections`.
- **Hashing**: `dict` and `set`, handling collisions using lists or linked lists.
- **Trees**: Binary trees, Binary Search Trees (BST), DFS, BFS, tree traversals.
- **Heaps**: Min-heap and max-heap using `heapq` module.
- **Graphs**: BFS, DFS, Dijkstra’s, Prim’s, Kruskal’s algorithms using adjacency lists.
- **Trie**: Implemented using `dict` for prefix trees.

## 2. Algorithms

- **Sorting Algorithms**: QuickSort, MergeSort, BubbleSort, HeapSort.
- **Searching Algorithms**: Binary search, linear search, BFS, DFS.
- **Recursion**: Backtracking, N-Queens, maze solving.
- **Dynamic Programming**: Knapsack, LCS, LIS, matrix chain multiplication.
- **Greedy Algorithms**: Activity selection, coin change, Huffman coding.
- **Divide and Conquer**: Merge sort, quick sort, binary search.
- **Graph Algorithms**: Dijkstra’s, Bellman-Ford, Floyd Warshall, Prim's, Kruskal’s.
- **Bit Manipulation**: XOR, AND, OR, shifting bits for optimizations.

## 3. Object-Oriented Programming (OOP)

- **Encapsulation, Inheritance, Polymorphism, Abstraction**: Implementing and understanding OOP concepts.
- **Design Patterns**: Singleton, Factory, Observer, Strategy patterns in Python.

## 4. Python-Specific Concepts

- **Exception Handling**: `try-except-finally` blocks, handling specific exceptions.
- **Concurrency and Multithreading**: `threading`, `multiprocessing`, GIL (Global Interpreter Lock).
- **Iterators and Generators**: Creating custom iterators and using `yield` for generators.
- **Decorators and Context Managers**: Using and creating decorators, `with` statement for context management.
- **Comprehensions**: List, dictionary, and set comprehensions for concise code.
- **Lambda and Higher-Order Functions**: Using `lambda`, `map`, `filter`, `reduce`.
  
## 5. Math and Number Theory

- **Prime Numbers**: Sieve of Eratosthenes, primality tests.
- **Greatest Common Divisor (GCD)**: Using `math.gcd` or Euclidean algorithm.
- **Modular Arithmetic**: Modular exponentiation, Fermat’s Little Theorem.
- **Combinatorics**: Factorial, combinations, permutations using `math.factorial` and `itertools`.
- **Number Theory**: Prime factorization, LCM, modular inverses.

## 6. Input/Output Optimization

- **Fast Input/Output**: Using `sys.stdin` and `sys.stdout` for faster input/output.
- **Efficient String Handling**: Use `join` for concatenation and f-strings for formatting.

## 7. Practice Platforms

- **LeetCode, Codeforces, HackerRank, CodeChef, GeeksforGeeks**: Platforms providing competitive programming problems in Python.

---

# Different Ways to Take User Input in Python

Python provides several ways to take user input, depending on the requirements.

## 1. Using `input()` Function

The simplest and most common way to take input from users.

```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))
print(f"Name: {name}, Age: {age}")
```

## 2. Using `sys.stdin` for Faster Input

For competitive programming, `sys.stdin` provides faster input reading than `input()`.

```python
import sys

name = sys.stdin.readline().strip()  # Reads a line and removes newline character
age = int(sys.stdin.readline().strip())
print(f"Name: {name}, Age: {age}")
```

## 3. Using Command Line Arguments

You can also take inputs via command line arguments using the `sys.argv` list.

```python
import sys

if len(sys.argv) < 3:
    print("Please provide name and age as command line arguments.")
else:
    name = sys.argv[1]
    age = int(sys.argv[2])
    print(f"Name: {name}, Age: {age}")
```

---

# Python Primitive Types - Range, Size, and Key Functions

| **Type**  | **Range**         | **Key Functions**                                       |
| --------- | ----------------- | ------------------------------------------------------ |
| `int`     | Arbitrary-precision| `+`, `-`, `*`, `//`, `%`, `**`                         |
| `float`   | ±1.7e−308 to ±1.7e+308 | `+`, `-`, `*`, `/`, `//`, `%`, `**`, `math.ceil()`, `math.floor()` |
| `bool`    | `True`, `False`    | Logical operators (`and`, `or`, `not`)                 |
| `str`     | Sequence of characters | Slicing, `len()`, `upper()`, `lower()`, `replace()`  |
| `list`    | Mutable sequence   | `append()`, `extend()`, `remove()`, `sort()`, slicing  |
| `tuple`   | Immutable sequence | Slicing, `index()`, `count()`                          |
| `dict`    | Key-value pairs    | `get()`, `keys()`, `values()`, `items()`, `update()`   |
| `set`     | Unordered collection | `add()`, `remove()`, `union()`,

 `intersection()`   |

---

# Python Mutable vs Immutable Types

## Key Mutable Types

- **List**
- **Dictionary**
- **Set**

## Key Immutable Types

- **int**
- **float**
- **bool**
- **str**
- **tuple**

---

# Python Strings - Common Methods

| **Method**                  | **Description**                                      |
| --------------------------- | ---------------------------------------------------- |
| `str.upper()`               | Converts all characters to uppercase.                |
| `str.lower()`               | Converts all characters to lowercase.                |
| `str.strip()`               | Removes leading and trailing whitespace.             |
| `str.replace(old, new)`     | Replaces occurrences of `old` substring with `new`.  |
| `str.split(delimiter)`      | Splits the string by the specified delimiter.        |
| `str.join(iterable)`        | Joins elements of an iterable with the string as separator. |
| `str.find(substring)`       | Returns the index of the first occurrence of a substring. |
| `str.count(substring)`      | Counts occurrences of a substring.                   |
| `str.isdigit()`             | Returns `True` if the string consists of digits only.|

## Additional Notes:

- Strings in Python are immutable, meaning they cannot be changed after creation.
- String formatting: Use f-strings (`f"{var}"`) for efficient and readable string formatting.

---

# Collections Framework in Python

## List

| **Method**                  | **Description**                                     |
| --------------------------- | --------------------------------------------------- |
| `append(item)`              | Adds an item to the end of the list.                |
| `insert(index, item)`       | Inserts an item at a specified index.               |
| `remove(item)`              | Removes the first occurrence of the item.           |
| `pop([index])`              | Removes and returns the item at the given index.    |
| `sort()`                    | Sorts the list in-place.                            |
| `reverse()`                 | Reverses the list in-place.                         |
| `extend(iterable)`          | Extends the list by appending elements from the iterable. |

## Set

| **Method**                  | **Description**                                     |
| --------------------------- | --------------------------------------------------- |
| `add(item)`                 | Adds an item to the set if it is not already present.|
| `remove(item)`              | Removes the specified item.                         |
| `union(other_set)`          | Returns a new set with elements from both sets.     |
| `intersection(other_set)`    | Returns a new set with elements common to both sets.|
| `difference(other_set)`     | Returns a new set with elements in the set but not in the other set. |

## Dictionary

| **Method**                  | **Description**                                     |
| --------------------------- | --------------------------------------------------- |
| `get(key, default)`         | Returns the value for the specified key or a default if not found.|
| `keys()`                    | Returns a view object of the dictionary's keys.     |
| `values()`                  | Returns a view object of the dictionary's values.   |
| `items()`                   | Returns a view object of the dictionary's key-value pairs. |
| `update(other_dict)`        | Updates the dictionary with the key-value pairs from another dictionary. |

## Tuple

| **Method**                  | **Description**                                     |
| --------------------------- | --------------------------------------------------- |
| `count(item)`               | Returns the number of times an item appears in the tuple. |
| `index(item)`               | Returns the index of the first occurrence of the item.|

## Deque

| **Method**                  | **Description**                                     |
| --------------------------- | --------------------------------------------------- |
| `append(item)`              | Appends an item to the right end of the deque.      |
| `appendleft(item)`          | Appends an item to the left end of the deque.       |
| `pop()`                     | Removes and returns the rightmost item.            |
| `popleft()`                 | Removes and returns the leftmost item.             |

## Heap (using `heapq`)

| **Method**                  | **Description**                                     |
| --------------------------- | --------------------------------------------------- |
| `heapify(list)`             | Converts a list into a heap.                        |
| `heappush(heap, item)`      | Pushes an item onto the heap.                       |
| `heappop(heap)`             | Pops and returns the smallest item from the heap.   |
| `heappushpop(heap, item)`   | Pushes and pops the smallest item simultaneously.   |

## Priority Queue

Priority queues can be implemented using `heapq` or `queue.PriorityQueue`.

| **Method**                  | **Description**                                     |
| --------------------------- | --------------------------------------------------- |
| `put(item)`                 | Puts an item into the priority queue.               |
| `get()`                     | Removes and returns the smallest item.             |

## Trie (using dictionary)

A simple implementation of a Trie using nested dictionaries:

```python
class TrieNode:
    def __init__(self):
        self.children = {}
        self.is_end_of_word = False

class Trie:
    def __init__(self):
        self.root = TrieNode()

    def insert(self, word):
        node = self.root
        for char in word:
            if char not in node.children:
                node.children[char] = TrieNode()
            node = node.children[char]
        node.is_end_of_word = True

    def search(self, word):
        node = self.root
        for char in word:
            if char not in node.children:
                return False
            node = node.children[char]
        return node.is_end_of_word
```

## Additional Notes:

- Python's `collections` module provides specialized container types such as `defaultdict`, `Counter`, and `OrderedDict`.

---

# Comparison of Python Collections

| **Collection Type** | **Add (Write)** | **Get (Read)** | **Remove (Delete)** | **Contains** | **Iteration** | **Memory Usage** | **Notes**                                   |
| ------------------- | --------------- | -------------- | ------------------- | ------------ | ------------- | ---------------- | ------------------------------------------- |
| **List**            | O(1)            | O(1)           | O(n)                | O(n)         | O(n)          | Moderate         | Fast random access, slow deletions.         |
| **Set**             | O(1)            | O(1)           | O(1)                | O(1)         | O(n)          | Low              | Unordered, no duplicates, fast lookups.     |
| **Dictionary**      | O(1)            | O(1)           | O(1)                | O(1)         | O(n)          | Moderate         | Key-value pairs, fast access and updates.   |
| **Tuple**           | O(1)            | O(1)           | Immutable           | O(n)         | O(n)          | Low              | Immutable sequence, lightweight.            |
| **Deque**           | O(1)            | O(n)           | O(1) (front/back)   | O(n)         | O(n)          | Moderate         | Fast insertions/removals at both ends.      |

## Additional Notes:

- **Memory Usage**: Depends on the collection type and number of elements.
- **Time Complexity**: Choose a data structure based on the operations you need to optimize.

---

# Python Math Library Functions

The Python `math` module provides a variety of mathematical functions.

| **Function**                | **Description**                                     |
| --------------------------- | --------------------------------------------------- |
| `math.sqrt(x)`              | Returns the square root of `x`.                     |
| `math.factorial(x)`         | Returns the factorial of `x`.                       |
| `math.gcd(x, y)`            | Returns the greatest common divisor of `x` and `y`. |
| `math.pow(x, y)`            | Returns `x` raised to the power `y`.                |
| `math.log(x, [base])`       | Returns the logarithm of `x` to the specified base. |
| `math.sin(x)`               | Returns the sine of `x` (in radians).               |
| `math.cos(x)`               | Returns the cosine of `x` (in radians).             |
| `math.tan(x)`               | Returns the tangent of `x` (in radians).            |
| `math.pi`                   | The constant π (3.14159…).                         |
| `math.e`                    | The constant e (2.71828…).                         |

---

# Python Arrays (using `array` module)

The `array` module provides space-efficient arrays of basic C-style types.

| **Method**                  | **Description**                                     |
| --------------------------- | --------------------------------------------------- |
| `array(typecode, iterable)` | Creates an array with the specified typecode and initializes it with elements from the iterable. |
| `append(item)`              | Appends an item to the array.                       |
| `extend(iterable)`          | Extends the array by appending elements from an iterable. |
| `pop([index])`              | Removes and returns the element at the specified index. |
| `index(item)`               | Returns the index of the first occurrence of the item. |

---

# Python List Comprehension and Generator Expressions

## List Comprehension

List comprehension provides a concise way to create lists.

```python
# Example: Creating a list of squares
squares = [x**2 for x in range(10)]
```

## Generator Expressions

Generator expressions are similar to list comprehensions but return a generator object.

```python
# Example: Creating a generator for squares


squares = (x**2 for x in range(10))
```

---

# Different Ways to Sort Collections in Python

## 1. Using `sort()` Method

The `sort()` method sorts the list in-place.

### Example:

```python
fruits = ["banana", "apple", "cherry"]
fruits.sort()
print(fruits)  # Output: ['apple', 'banana', 'cherry']
```

## 2. Using `sorted()` Function

The `sorted()` function returns a new sorted list without modifying the original list.

### Example:

```python
fruits = ["banana", "apple", "cherry"]
sorted_fruits = sorted(fruits)
print(sorted_fruits)  # Output: ['apple', 'banana', 'cherry']
```

## 3. Sorting with Lambda Functions

You can use lambda functions for custom sorting criteria.

### Example:

```python
fruits = ["banana", "apple", "cherry"]
fruits.sort(key=lambda fruit: len(fruit))
print(fruits)  # Output: ['apple', 'banana', 'cherry']
```

---

# Summary of Sorting Approaches in Python

## 1. Using `sort()` Method

- **Description**: In-place sorting of lists.
- **Use Case**: When you want to modify the list in-place.

## 2. Using `sorted()` Function

- **Description**: Returns a new sorted list without modifying the original.
- **Use Case**: When you need the original list unmodified.

## 3. Sorting with Lambda Functions

- **Description**: Custom sorting logic using lambda expressions.
- **Use Case**: When you need a specific sorting order based on custom criteria.

These methods offer flexibility for sorting various data types and structures in Python.