- [1. **JavaScript Basics**](#1-javascript-basics)
- [2. **Functions**](#2-functions)
- [3. **Objects and Arrays**](#3-objects-and-arrays)
- [4. **Asynchronous JavaScript**](#4-asynchronous-javascript)
- [5. **Event Handling**](#5-event-handling)
- [6. **JavaScript ES6+ Features**](#6-javascript-es6-features)
- [7. **Scope and Hoisting**](#7-scope-and-hoisting)
- [8. **DOM and Browser APIs**](#8-dom-and-browser-apis)
- [9. **Error Handling**](#9-error-handling)
- [10. **Common Data Structures**](#10-common-data-structures)
- [11. **Object-Oriented JavaScript**](#11-object-oriented-javascript)
- [12. **Memory Management**](#12-memory-management)
- [13. **Testing and Debugging**](#13-testing-and-debugging)
- [14. **Common Patterns and Best Practices**](#14-common-patterns-and-best-practices)
- [15. **Miscellaneous Topics**](#15-miscellaneous-topics)
- [16. Detailed Explanation of Common Data Structures in JavaScript](#16-detailed-explanation-of-common-data-structures-in-javascript)
  - [1. **Arrays**](#1-arrays)
  - [2. **Objects (Hash Maps/Hash Tables)**](#2-objects-hash-mapshash-tables)
  - [3. **Sets**](#3-sets)
  - [4. **Maps**](#4-maps)
  - [5. **Stacks**](#5-stacks)
  - [6. **Queues**](#6-queues)
  - [7. **Linked Lists**](#7-linked-lists)
- [17. Relevant Topics for Competitive Programming](#17-relevant-topics-for-competitive-programming)
  - [1. **Dynamic Programming (DP)**](#1-dynamic-programming-dp)
  - [2. **Greedy Algorithms**](#2-greedy-algorithms)
  - [3. **Backtracking**](#3-backtracking)
  - [4. **Graph Algorithms**](#4-graph-algorithms)
  - [5. **Sorting and Searching**](#5-sorting-and-searching)
- [Conclusion](#conclusion)

### 1. **JavaScript Basics**

**Data Types:**
JavaScript has several primitive data types: `String`, `Number`, `Boolean`, `undefined`, `null`, `Symbol`, and `BigInt`.

```js
let str = "Hello"; // String
let num = 42; // Number
let bool = true; // Boolean
let notDefined; // undefined
let empty = null; // null
let bigInt = 123n; // BigInt
```

**Variables:**

- `var`: function-scoped and can be re-declared.
- `let`: block-scoped and cannot be re-declared within the same scope.
- `const`: block-scoped and cannot be re-assigned.

```js
var x = 10;
let y = 20;
const z = 30;
```

**Operators:**

- Arithmetic: `+`, `-`, `*`, `/`, `%`
- Logical: `&&`, `||`, `!`
- Comparison: `==`, `===`, `!=`, `!==`, `>`, `<`, `>=`, `<=`

```js
let a = 5,
  b = 10;
console.log(a + b); // 15 (Arithmetic)
console.log(a > b); // false (Comparison)
console.log(a && b); // 10 (Logical)
```

**Type Coercion:**
Implicit and explicit conversion between types.

```js
console.log("5" + 1); // "51" (String concatenation)
console.log(Number("5") + 1); // 6 (Explicit coercion)
```

---

### 2. **Functions**

**Function Declaration vs Expression:**

- Declaration: can be hoisted.
- Expression: cannot be hoisted.

```js
function add(a, b) {
  return a + b;
} // Declaration
let subtract = function (a, b) {
  return a - b;
}; // Expression
```

**Arrow Functions:**
A shorter syntax for functions that also preserves the `this` context.

```js
let multiply = (a, b) => a * b;
```

**Higher-order Functions:**
Functions that take other functions as arguments or return functions.

```js
function higherOrder(fn, value) {
  return fn(value);
}
console.log(higherOrder((x) => x * 2, 5)); // 10
```

**Closures:**
Functions that "remember" the variables from their scope even when called outside of that scope.

```js
function outer() {
  let count = 0;
  return function () {
    return ++count;
  };
}
let counter = outer();
console.log(counter()); // 1
console.log(counter()); // 2
```

**Recursion:**
A function that calls itself.

```js
function factorial(n) {
  if (n === 0) return 1;
  return n * factorial(n - 1);
}
console.log(factorial(5)); // 120
```

---

### 3. **Objects and Arrays**

**Objects:**
Collections of key-value pairs.

```js
let person = { name: "John", age: 30 };
console.log(person.name); // "John"
```

**Array Methods:**

- `map()`: Applies a function to each element.
- `filter()`: Filters elements based on a condition.
- `reduce()`: Reduces the array to a single value.

```js
let arr = [1, 2, 3, 4];
let doubled = arr.map((x) => x * 2); // [2, 4, 6, 8]
let even = arr.filter((x) => x % 2 === 0); // [2, 4]
let sum = arr.reduce((acc, curr) => acc + curr, 0); // 10
```

**Destructuring:**
Extract values from objects or arrays into variables.

```js
let { name, age } = person; // Destructuring object
let [first, second] = arr; // Destructuring array
```

**Spread/Rest Operators:**

- Spread: Expands an array/object into its elements.
- Rest: Collects arguments into an array.

```js
let arr2 = [...arr, 5, 6]; // Spread
function sumAll(...numbers) {
  return numbers.reduce((a, b) => a + b);
} // Rest
```

**Prototypes:**
Objects inherit properties and methods from their prototype.

```js
function Animal(type) {
  this.type = type;
}
Animal.prototype.speak = function () {
  return "I am a " + this.type;
};
let dog = new Animal("dog");
console.log(dog.speak()); // "I am a dog"
```

---

### 4. **Asynchronous JavaScript**

**Promises:**
Handles asynchronous operations.

```js
let promise = new Promise((resolve, reject) => {
  setTimeout(() => resolve("Done!"), 1000);
});
promise.then((result) => console.log(result)); // "Done!" after 1 second
```

**Async/Await:**
Syntax for handling Promises more cleanly.

```js
async function fetchData() {
  let result = await fetch("https://api.example.com");
  let data = await result.json();
  console.log(data);
}
fetchData();
```

**Event Loop:**
JavaScript uses an event loop to handle asynchronous operations and execute tasks.

```js
console.log("Start");
setTimeout(() => console.log("Inside Timeout"), 0);
console.log("End");
```

---

### 5. **Event Handling**

**Event Listeners:**
Adding events to DOM elements.

```js
document.getElementById("myBtn").addEventListener("click", function () {
  alert("Button clicked");
});
```

**Event Delegation:**
Attaching a single event handler for multiple child elements using event propagation.

```js
document.querySelector("ul").addEventListener("click", function (e) {
  if (e.target.tagName === "LI") {
    console.log("List item clicked: " + e.target.textContent);
  }
});
```

---

### 6. **JavaScript ES6+ Features**

**Template Literals:**
Allows embedding variables in strings using backticks.

```js
let name = "Alice";
console.log(`Hello, ${name}`); // "Hello, Alice"
```

**Default Parameters:**
Default values for function parameters.

```js
function greet(name = "Guest") {
  console.log("Hello, " + name);
}
greet(); // "Hello, Guest"
```

**Classes:**
JavaScript `class` syntax to define objects.

```js
class Animal {
  constructor(type) {
    this.type = type;
  }
  speak() {
    return "I am a " + this.type;
  }
}
let cat = new Animal("cat");
console.log(cat.speak()); // "I am a cat"
```

---

### 7. **Scope and Hoisting**

**Scope:**

- `let` and `const` are block-scoped.
- `var` is function-scoped.

```js
if (true) {
  let x = 10;
  var y = 20;
}
console.log(y); // 20
console.log(x); // Error: x is not defined
```

**Hoisting:**
Variable declarations (not initializations) and function declarations are moved to the top of their scope.

```js
console.log(a); // undefined
var a = 5;
```

---

### 8. **DOM and Browser APIs**

**DOM Manipulation:**

- Accessing and modifying elements.

```js
let element = document.getElementById("myElement");
element.textContent = "New Content";
```

**Browser APIs:**

- `fetch()`: Make HTTP requests.
- `localStorage`/`sessionStorage`: Store data locally.

```js
localStorage.setItem("name", "Alice");
let name = localStorage.getItem("name");
```

---

### 9. **Error Handling**

**`try`, `catch`, `finally`:**
Handle exceptions in JavaScript.

```js
try {
  let x = y + 1; // y is not defined
} catch (error) {
  console.log("Error:", error.message);
} finally {
  console.log("This runs no matter what");
}
```

---

### 10. **Common Data Structures**

**Sets:**
A collection of unique values.

```js
let set = new Set([1, 2, 3, 4, 5]);
set.add(3); // Set remains the same (no duplicates)
```

**Maps:**
A collection of key-value pairs.

```js
let map = new Map();
map.set("name", "Alice");
console.log(map.get("name")); // "Alice"
```

---

### 11. **Object-Oriented JavaScript**

**Class Inheritance:**

```js
class Animal {
  constructor(type) {
    this.type = type;
  }
  speak() {
    return "I am a " + this.type;
  }
}
class Dog extends Animal {
  speak() {
    return super.speak() + " and I bark";
  }
}
let dog = new Dog("dog");
console.log(dog.speak()); // "I am a dog and I bark"
```

---

### 12. **Memory Management**

**Garbage Collection:**
JavaScript automatically frees up memory that is no longer in use.

```js
let obj = { name: "Alice" };
obj = null; // Eligible for garbage collection
```

---

### 13. **Testing and Debugging**

**Unit Testing:**
Example with Jest:

```js
test("adds 1 + 2 to equal 3", () => {
  expect(1 + 2).toBe(3);
});
```

**Debugging Tools:**
Use browser DevTools to debug.

```js
console.log("Debugging info");
```

---

### 14. **Common Patterns and Best Practices**

**Module Pattern:**
Encapsulate functionality to maintain a clean code structure.

```js
const module = (function () {
  let privateVar = "I'm private";
  return {
    publicMethod: function () {
      return privateVar;
    },
  };
})();
console.log(module.publicMethod()); // "I'm private"
```

---

### 15. **Miscellaneous Topics**

**JSON Manipulation:**

```js
let obj = { name: "Alice" };
let jsonString = JSON.stringify(obj);
let parsedObj = JSON.parse(jsonString);
```

**CORS:**
Cross-Origin Resource Sharing enables access to resources on different domains while ensuring security policies.

---

### 16. Detailed Explanation of Common Data Structures in JavaScript

In competitive programming, data structures play a key role in solving problems efficiently. Here’s a detailed breakdown of common data structures in JavaScript, their usage, and examples:

---

#### 1. **Arrays**

Arrays are ordered collections that store values (indexed starting from 0). They are one of the most commonly used data structures in competitive programming.

**Common Methods:**

- `push()`: Adds an element to the end.
- `pop()`: Removes the last element.
- `shift()`: Removes the first element.
- `unshift()`: Adds an element to the start.
- `slice()`: Returns a portion of an array.
- `splice()`: Modifies an array by adding/removing elements.

**Example Usage:**

```js
let arr = [1, 2, 3, 4];
arr.push(5); // [1, 2, 3, 4, 5]
arr.pop(); // [1, 2, 3, 4]
arr.shift(); // [2, 3, 4]
arr.unshift(0); // [0, 2, 3, 4]
let newArr = arr.slice(1, 3); // [2, 3]
```

**Time Complexity:**

- Access: O(1)
- Search: O(n)
- Insertion/Deletion at the end: O(1)
- Insertion/Deletion at the beginning: O(n)

---

#### 2. **Objects (Hash Maps/Hash Tables)**

Objects in JavaScript function as hash maps. They store key-value pairs and offer fast access, insertion, and deletion.

**Common Methods:**

- `Object.keys()`: Returns an array of an object’s keys.
- `Object.values()`: Returns an array of an object’s values.
- `delete`: Removes a property from an object.

**Example Usage:**

```js
let obj = { name: "Alice", age: 25, city: "New York" };
console.log(obj.name); // Access: "Alice"
delete obj.age; // Removes the age property
console.log(obj); // { name: "Alice", city: "New York" }
```

**Time Complexity:**

- Access: O(1)
- Search: O(1)
- Insertion/Deletion: O(1)

**Use Cases:**

- Counting frequencies of elements.
- Storing memoization data.

---

#### 3. **Sets**

A `Set` is a collection of unique values. It helps in scenarios where duplicate elements should be avoided.

**Common Methods:**

- `add()`: Adds an element to the set.
- `has()`: Checks if an element exists in the set.
- `delete()`: Removes an element from the set.
- `size`: Returns the number of elements.

**Example Usage:**

```js
let set = new Set([1, 2, 3, 4, 5]);
set.add(6); // Adds 6
console.log(set.has(3)); // true
set.delete(1); // Removes 1
console.log(set.size); // 5
```

**Time Complexity:**

- Access: O(n)
- Search: O(1)
- Insertion/Deletion: O(1)

**Use Cases:**

- Removing duplicates from an array.
- Checking for membership in constant time.

---

#### 4. **Maps**

`Map` is an ordered collection of key-value pairs. Unlike objects, keys in a map can be of any type (including functions, objects, etc.).

**Common Methods:**

- `set()`: Adds or updates an element.
- `get()`: Retrieves an element by key.
- `delete()`: Removes an element by key.
- `has()`: Checks if a key exists.
- `size`: Returns the number of elements.

**Example Usage:**

```js
let map = new Map();
map.set("name", "Alice");
map.set("age", 25);
console.log(map.get("name")); // "Alice"
map.delete("age");
console.log(map.size); // 1
```

**Time Complexity:**

- Access: O(1)
- Search: O(1)
- Insertion/Deletion: O(1)

---

#### 5. **Stacks**

A `Stack` is a last-in-first-out (LIFO) data structure. Stacks are used in scenarios where you need to reverse things or track history (e.g., undo/redo operations).

**Operations:**

- `push()`: Adds an element to the top of the stack.
- `pop()`: Removes and returns the top element.
- `peek()`: Returns the top element without removing it.
- `isEmpty()`: Checks if the stack is empty.

**Example Usage:**

```js
class Stack {
  constructor() {
    this.items = [];
  }
  push(item) {
    this.items.push(item);
  }
  pop() {
    return this.items.pop();
  }
  peek() {
    return this.items[this.items.length - 1];
  }
  isEmpty() {
    return this.items.length === 0;
  }
}

let stack = new Stack();
stack.push(10);
stack.push(20);
console.log(stack.peek()); // 20
stack.pop(); // Removes 20
console.log(stack.isEmpty()); // false
```

**Time Complexity:**

- Access/Search: O(n)
- Insertion/Deletion: O(1)

---

#### 6. **Queues**

A `Queue` is a first-in-first-out (FIFO) data structure, often used for scheduling and processing tasks in order.

**Operations:**

- `enqueue()`: Adds an element to the back.
- `dequeue()`: Removes and returns the front element.
- `peek()`: Returns the front element without removing it.
- `isEmpty()`: Checks if the queue is empty.

**Example Usage:**

```js
class Queue {
  constructor() {
    this.items = [];
  }
  enqueue(item) {
    this.items.push(item);
  }
  dequeue() {
    return this.items.shift();
  }
  peek() {
    return this.items[0];
  }
  isEmpty() {
    return this.items.length === 0;
  }
}

let queue = new Queue();
queue.enqueue(1);
queue.enqueue(2);
console.log(queue.peek()); // 1
queue.dequeue(); // Removes 1
console.log(queue.isEmpty()); // false
```

**Time Complexity:**

- Access/Search: O(n)
- Insertion/Deletion: O(1)

---

#### 7. **Linked Lists**

A `Linked List` is a linear data structure where each element (node) contains a reference to the next element in the sequence. This is useful for dynamic memory allocation and when frequent insertions or deletions are required.

**Operations:**

- Insert: O(1) at the head or tail.
- Delete: O(n).
- Traverse: O(n).

**Example Usage:**

```js
class Node {
  constructor(value) {
    this.value = value;
    this.next = null;
  }
}

class LinkedList {
  constructor() {
    this.head = null;
  }

  append(value) {
    let newNode = new Node(value);
    if (!this.head) {
      this.head = newNode;
    } else {
      let current = this.head;
      while (current.next) {
        current = current.next;
      }
      current.next = newNode;
    }
  }

  print() {
    let current = this.head;
    while (current) {
      console.log(current.value);
      current = current.next;
    }
  }
}

let list = new LinkedList();
list.append(10);
list.append(20);
list.print(); // Outputs: 10 20
```

---

### 17. Relevant Topics for Competitive Programming

#### 1. **Dynamic Programming (DP)**

DP is a method for solving problems by breaking them into overlapping subproblems. It is often used for optimization problems.

**Example Problem: Fibonacci Sequence**

```js
function fibonacci(n, memo = {}) {
  if (n <= 1) return n;
  if (n in memo) return memo[n];
  memo[n] = fibonacci(n - 1, memo) + fibonacci(n - 2, memo);
  return memo[n];
}
console.log(fibonacci(10)); // 55
```

#### 2. **Greedy Algorithms**

Greedy algorithms make the optimal choice at each step. They work well for problems where local optima lead to a global solution.

**Example Problem: Coin Change**

```js
function coinChange(coins, amount) {
  let count = 0;
  coins.sort((a, b) => b - a); // Sort coins in descending order
  for (let coin of coins) {
    count += Math.floor(amount / coin);
    amount %= coin;
  }
  return amount === 0 ? count : -1;
}
console.log(coinChange([1, 2, 5], 11)); // 3 (5 + 5 + 1)
```

#### 3. **Backtracking**

Backtracking is used to solve constraint satisfaction problems by trying different solutions and undoing choices when they don't lead to a solution.

**Example Problem: N-Queens**

```js
function solveNQueens(n) {
  let result = [];
  function solve(row, cols, diags, antiDiags) {
    if (row === n) {
      result.push(cols.map((c) => ".".repeat(c) + "Q" + ".".repeat(n - c - 1)));
      return;
    }
    for (let col = 0; col < n; col++) {
      if (
        cols.includes(col) ||
        diags.includes(row - col) ||
        antiDiags.includes(row + col)
      )
        continue;
      solve(
        row + 1,
        [...cols, col],
        [...diags, row - col],
        [...antiDiags, row + col]
      );
    }
  }
  solve(0, [], [], []);
  return result;
}
console.log(solveNQueens(4)); // Solutions to 4-queens problem
```

#### 4. **Graph Algorithms**

Graphs are used to model relationships between elements, with common operations including depth-first search (DFS) and breadth-first search (BFS).

**Example: DFS**

```js
function dfs(graph, node, visited = new Set()) {
  if (visited.has(node)) return;
  console.log(node);
  visited.add(node);
  for (let neighbor of graph[node]) {
    dfs(graph, neighbor, visited);
  }
}
let graph = { 1: [2, 3], 2: [4], 3: [4], 4: [] };
dfs(graph, 1); // 1 2 4 3
```

#### 5. **Sorting and Searching**

Efficient sorting (like merge sort and quick sort) and binary search are crucial for solving many competitive problems.

**Example: Binary Search**

```js
function binarySearch(arr, target) {
  let left = 0,
    right = arr.length - 1;
  while (left <= right) {
    let mid = Math.floor((left + right) / 2);
    if (arr[mid] === target) return mid;
    else if (arr[mid] < target) left = mid + 1;
    else right = mid - 1;
  }
  return -1;
}
console.log(binarySearch([1, 2, 3, 4, 5], 3)); // 2
```

### Conclusion

Mastering these data structures and algorithms is crucial for success in competitive programming and technical interviews. Each data structure has specific use cases, time complexities, and can help solve a variety of problems more efficiently.
