
# Variables and Strings


## Introduction to JavaScript

## What Is JavaScript, and How Does It Work with HTML and CSS?

### Questions
---
**What role does JavaScript play in web development compared to HTML and CSS?**

- [ ] JavaScript provides structure to the webpage and ensures that your code is free of errors.
- [ ] JavaScript provides the styles for the web page and automatically formats your code.
- [X] JavaScript provides interactive functionality and dynamic behavior for the web page.
- [ ] JavaScript is only used to create advanced animations for web applications.

**Correct answer:** JavaScript provides interactive functionality and dynamic behavior for the web page.

---

**How does JavaScript typically interact with HTML and CSS on a webpage?**

- [ ] JavaScript adds more styles to the CSS file and more elements to the HTML file.
- [ ] JavaScript creates a new version of HTML for the page so your HTML code will run faster.
- [X] JavaScript interacts with the page to change content and styles dynamically.
- [ ] JavaScript only works in the back-end and is rarely used in the front-end.

**Correct answer:** JavaScript interacts with the page to change content and styles dynamically.

---

**Which of the following is true about the relationship between JavaScript, HTML, and CSS?**

- [ ] HTML is a programming language and CSS is a stylesheet language, while JavaScript is a markup language.
- [X] HTML is a markup language and CSS is a stylesheet language, while JavaScript is a programming language.
- [ ] JavaScript can replace HTML and CSS.
- [ ] JavaScript does not work with HTML and CSS.

**Correct answer:** HTML is a markup language and CSS is a stylesheet language, while JavaScript is a programming language.
---

## What Is a Data Type, and What Are the Different Data Types in JavaScript?

JavaScript has several different data types. A data type determines what kind of value a variable contains.

The first data type we will look at is the **Number** type.

```
let age = 25; // integer
let price = 19.99; // decimal or floating number
```

 The next data type is a **String**. A String represents text.

```
let name = 'Tarek'; // Single quotes
let message = "Hello World"; // double quotes
```

Another data type used in JavaScript is the **Boolean** type. A Boolean can have only two values: `true` or `false`.

```
let isStudent = true;
let isLoggedIn = false;
```

 The next two data types used in JavaScript are **undefined** and **null**.

 `undefined` means a variable has been declared but hasn't been given a value yet.

```
let city;

console.log(city); // undefined
```

 `null` means the variable has been intentionally set to "nothing" and does not hold any value.

```
let result = null;

console.log(result); // null
```

 The last three data types are more complex in nature. These are **Object, Symbol, and BigInt**.

 An **Object** is a collection of key-value pairs.

```
let person = {
  name: "Tarek",
  age: 25
};
```

 A **Symbol** is a primitive data type used to create unique values.

```
let id = Symbol("id");
```

 **BigInt** is used to represent very large integers.

```
let bigNumber = 12345678901234567890n; // adding n a the end
```

 ### Primitive Types

 The seven primitive data types in JavaScript are:

- `String`
- `Number`
- `BigInt`
- `Boolean`
- `Undefined`
- `Null`
- `Symbol`

 ### Non-Primitive Type

 The main non-primitive type is:

 - `Object`
  - Arrays
  - Functions
  - Objects

 ### Checking the Data Type with `typeof`

 To check the type of a value, we generally use the `typeof` operator.

```
console.log(typeof "Hello");        // "string"
console.log(typeof 42);             // "number"
console.log(typeof true);           // "boolean"
console.log(typeof undefined);      // "undefined"
console.log(typeof {});             // "object"
```

 ### Quick Summary

| Data Type | Example |
| --- | --- |
| String | `"Hello"` |
| Number | `42` |
| BigInt | `123n` |
| Boolean | `true` |
| Undefined | `undefined` |
| Null | `null` |
| Symbol | `Symbol("id")` |
| Object | `{ name: "Tarek" }` |



### Questions
---
**Which of the following is a string data type?**

- [X] "Hello!"
- 42
- false
- null
---
**What data type represents a value that is either true or false?**
- Number
- String
- [X] Boolean
- undefined
---
**If a variable has been declared but not assigned a value, what is its data type?**
- String
- Number
- [X] undefined
- null
---
## What Are Variables, and What Are Guidelines for Naming JavaScript Variables?

### Declaring a Variable with let
```
let age;
console.log(age); // undefined
```

### Rules for Variable Names
Variables in JavaScript must begin with a letter, an underscore (_), or a dollar sign ($). They cannot start with a number.

```
// Valid variable names
let age;
let _score;
let $total;
let thisIsCamelCase;

// Invalid variable names
let 1stPlace; // starts with a number
```

Reserved Keywords and Special Characters such as let, const, function, or return, as they are reserved for the language itself.

### Questions
---
**Which keyword would you use to declare a variable in JavaScript when you plan to update its value later?**
- set
- [X] let
- declare
- variable
---
**Which of the following is a valid variable name in JavaScript?**
- 1stPlace
- total-score!
- [X] player1Score
- const
---
**Why is it important to use descriptive names for your variables?**
- It's required by JavaScript.
- [X] Descriptive names make your code easier to understand and maintain.
- Descriptive names make the code run faster.
- Descriptive names allow you to avoid using let.

---
## How Do let and const Work Differently When It Comes to Variable Declaration, Assignment, and Reassignment?

- You should use let when you need to declare variables that will be reassigned later. 


- Use const when you want to declare variables that should remain constant, like configuration values or settings that shouldn't be changed accidentally.

- You can also use the var keyword, but it's not as recommended anymore. The var keyword is kind of like let, except it has a wider scope, which is more likely to cause problems in your program.

```
let age = 25;
console.log(age) // 25
let age = 90; // SyntaxError: Identifier 'age' has already been declared


const maxScore; // Error: Missing initializer in const declaration

const maxScore = 100;
console.log(maxScore); // 100
maxScore = 200; // This will result in an error
```

### Questions
---

**What happens if you try to reassign a value to a variable declared with const?**

- The value will change without issue.
- The original value will be updated, but a warning will be issued.
- [X] An error will be thrown because const variables cannot be reassigned.
- The new value will be ignored, and the original value will stay the same.
---

**Which of the following is the correct way to assign the number 100 to a constant named maxScore?**
- const maxScore === 100;
- [X] const maxScore = 100;
- const maxScore <= 100;
- const maxScore == 100;

---

**Can you declare a const variable without assigning it a value?**
- Yes, but you must assign a value later.
- [X] No, const variables must be initialized at the time of declaration.
- Yes, but you can only assign a number as the initial value.
- No, const variables must be declared and reassigned in the same line.

---