# Welcome to the JavaScript Interview Questions & Answers repository!

This repository is a comprehensive collection of JavaScript interview questions and answers designed to help you prepare for your next tech interview. Whether you're a beginner or an experienced developer, you'll find valuable insights and resources to sharpen your JavaScript skills and boost your confidence.

## What's Inside

- Detailed Q&A: In-depth questions and answers covering all aspects of JavaScript.
- Concept Explanations: Clear explanations of fundamental and advanced JavaScript concepts.
- Code Examples: Practical examples to help you understand and apply JavaScript concepts.
- Interview Tips: Best practices and tips for acing your JavaScript interviews.

## How to Use

- Browse through the questions and answers to study and understand key JavaScript topics.
- Use the code examples to practice and solidify your knowledge.
- Follow the interview tips to improve your interview performance.

## Contributing

We welcome contributions! If you have any JavaScript interview questions or answers that you'd like to share, please feel free to open an issue or submit a pull request.

Happy coding and good luck with your interviews!

# Table of Contents

| No. | Title                                                          | Show Answer                                                                                                                                  |
| --- | -------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | What is JavaScript?                                            | <details><summary><strong><a href="#javascript-overview" style="text-decoration: none; color: blue;">Show Answer</a></strong></summary><br>  |
| 2   | Where can I use JavaScript?                                    | <details><summary><strong><a href="#usage" style="text-decoration: none; color: blue;">Show Answer</a></strong></summary><br>                |
| 3   | Which libraries and frameworks are built in JavaScript?        | <details><summary><strong><a href="#libraries-frameworks" style="text-decoration: none; color: blue;">Show Answer</a></strong></summary><br> |
| 4   | What are primitive and non-primitive data types in JavaScript? | <details><summary><strong><a href="#data-types" style="text-decoration: none; color: blue;">Show Answer</a></strong></summary><br>           |
| 5   | Understanding References in JavaScript                         | <details><summary><strong><a href="#references-types" style="text-decoration: none; color: blue;">Show Answer</a></strong></summary><br>     |

---

## 1. What is JavaScript?

<a name="javascript-overview"></a>

JavaScript is a versatile, high-level programming language primarily used for adding interactivity to web pages. It operates as an interpreted language, executing code line by line without prior compilation.

### Historical Context

JavaScript was created by Brendan Eich in 1995 while he was at Netscape Communications Corporation. Originally named "Mocha" and later "LiveScript," it was rebranded as JavaScript to align with the popularity of Java.

### Key Features

- **Dynamic Typing:** Variables can hold values of any data type without explicit declarations.
- **Prototype-based Object Orientation:** Objects inherit properties and behaviors from prototypes.

- **Functional Programming Support:** Functions are treated as first-class citizens, enabling higher-order functions and closures.

[Move to Top](#table-of-contents)

---

## 2. Where can I use JavaScript?

<a name="usage"></a>

JavaScript can be used for both client-side and server-side development. It's integral to creating interactive web pages, developing web and mobile applications, building APIs, and even for server-side programming using platforms like Node.js.

[Move to Top](#table-of-contents)

---

## 3. Which libraries and frameworks are built in JavaScript?

<a name="libraries-frameworks"></a>

JavaScript has a rich ecosystem of libraries and frameworks that simplify and enhance development. Some popular examples include:

- **React.js:** A JavaScript library for building user interfaces.
- **AngularJS and Angular:** Frameworks for building web applications.

- **Node.js:** A runtime environment that allows JavaScript to run server-side.

These tools and frameworks extend JavaScript's capabilities beyond basic scripting, enabling robust application development across various platforms.

[Move to Top](#table-of-contents)

---

## 4. What are primitive and non-primitive data types in JavaScript?

<a name="data-types"></a>

JavaScript supports different data types, categorized into primitive and non-primitive types.

- Primitive data: Primitive data types in JavaScript are immutable (unchangeable) and are directly operated upon by the language. They are stored directly in the variable's memory and are accessed by value.

| Data Type   | Description                                              | Example                        |
| ----------- | -------------------------------------------------------- | ------------------------------ |
| `number`    | Represents numeric data.                                 | `let count = 10;`              |
| `string`    | Represents textual data.                                 | `let message = 'Hello';`       |
| `boolean`   | Represents logical values.                               | `let isValid = true;`          |
| `null`      | Represents intentional absence of any object value.      | `let data = null;`             |
| `undefined` | Represents a variable declared but not assigned a value. | `let status;`                  |
| `symbol`    | Represents a unique identifier.                          | `const id = Symbol('unique');` |

- Non-primitive: Non-primitive data types are mutable (changeable) and are not stored directly in the variable's allocated memory. Instead, they are stored as references, and accessing these variables points to the reference in memory.

| Data Type  | Description                                    | Example                                             |
| ---------- | ---------------------------------------------- | --------------------------------------------------- |
| `object`   | Represents a collection of key-value pairs.    | `let person = { name: 'John', age: 30 };`           |
| `array`    | Represents a list-like collection of elements. | `let numbers = [1, 2, 3, 4, 5];`                    |
| `function` | Represents a reusable block of code.           | `function greet(name) { return 'Hello, ' + name; }` |

[Move to Top](#table-of-contents)

---

## Understanding References in JavaScript.

<a name="references-types"></a>

In JavaScript, references play a crucial role in how non-primitive data types are managed in memory. Unlike primitive data types (like numbers and strings) that are stored directly in the variable's location, non-primitive types (such as objects, arrays, and functions) are stored as references.

### How References Work

When you create a non-primitive data type, what actually gets stored in the variable is a reference to the memory location where the data is stored, rather than the data itself. This means:

1. **Reference to Memory:** Variables holding non-primitive types don't contain the actual data values but rather pointers or references to where the data resides in memory.

2. **Passing by Reference:** When you assign a non-primitive variable to another variable or pass it as an argument to a function, you're passing around this reference. This allows multiple variables to point to the same underlying data structure.

3. **Mutability:** Non-primitive types are mutable because you can change their properties or elements through their references. Modifying an object's property or adding/removing elements from an array affects the referenced data directly.

### Benefits of Reference-Based Storage

- **Memory Efficiency:** References enable efficient memory usage because you're not duplicating large data structures every time you assign or pass them.

- **Flexibility:** Referencing allows for complex data structures and dynamic changes without heavy memory overhead. This flexibility is crucial in modern JavaScript applications, where objects and arrays are commonly used to represent complex data relationships.

### Example

<!-- ```javascript -->

// Example of referencing in JavaScript

// Object creation
let person1 = { name: 'John', age: 30 };

// person2 references the same object as person1
let person2 = person1;

// Modifying person2 affects the referenced object
person2.age = 35;

console.log(person1.age); // Output: 35 (because person1 and person2 point to the same object)

[Move to Top](#table-of-contents)

---
