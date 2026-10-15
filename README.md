<div align="center">

# 🚀 JavaScript Interview Questions & Answers

### 💛 Top 100 JavaScript Interview Questions | Beginner to Advanced

![JavaScript](https://img.shields.io/badge/JavaScript-Modern-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Questions](https://img.shields.io/badge/Questions-100-2563EB?style=for-the-badge)
![Level](https://img.shields.io/badge/Level-Beginner%20to%20Advanced-16A34A?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

### 📚 Learn JavaScript | Practice JavaScript | Crack Interviews

**A complete JavaScript interview preparation guide with 100 carefully selected questions, easy-to-understand explanations, and practical code examples.**



### 👨‍💻 Created & Maintained By

**Jamshed Ahmad**

💻 **Code With Jamshed**

*Helping developers learn programming, improve problem-solving skills, and prepare for technical interviews.*

[![GitHub](https://img.shields.io/badge/GitHub-Jamshed7664-181717?style=for-the-badge&logo=github)](https://github.com/Jamshed7664)

⭐ **If you find this repository helpful, don't forget to give it a star!**

**Made with ❤️ by Jamshed Ahmad | Happy Coding! 🚀**

</div>

---

## 📖 About This Repository

This repository contains **100 JavaScript interview questions** with **short, beginner-friendly answers in simple Indian English**, plus practical code samples. It covers fundamentals, functions, objects, arrays, async JavaScript, browser concepts, and advanced topics.

> **How to study:** Read the question → understand the explanation → run the example → explain it in your own words. Browser-only examples need a web page/DevTools; other examples can run in Node.js.

## 🧭 Quick Navigation

- [1. JavaScript Fundamentals (Q1–Q18)](#section-1)
- [2. Functions, Scope & Closures (Q19–Q36)](#section-2)
- [3. Arrays, Strings & Objects (Q37–Q54)](#section-3)
- [4. Asynchronous JavaScript & Event Loop (Q55–Q72)](#section-4)
- [5. DOM, Browser & Events (Q73–Q81)](#section-5)
- [6. Objects, Prototypes & Advanced Concepts (Q82–Q100)](#section-6)

## 📊 Topic Breakdown

| Topic | Questions | Difficulty |
|:--|:--:|:--|
| JavaScript Fundamentals | 18 | Beginner |
| Functions, Scope & Closures | 18 | Beginner → Intermediate |
| Arrays, Strings & Objects | 18 | Beginner → Intermediate |
| Asynchronous JavaScript & Event Loop | 18 | Intermediate → Advanced |
| DOM, Browser & Events | 9 | Intermediate → Advanced |
| Objects, Prototypes & Advanced Concepts | 19 | Intermediate → Advanced |
| **Total** | **100** | **Beginner → Advanced** |

---

<a id="section-1"></a>
## 1. JavaScript Fundamentals

<details open>
<summary><strong>Expand / collapse questions</strong></summary>

### Q1. What is JavaScript?

**✅ Easy Explanation:** JavaScript is a programming language used to make websites interactive. It also runs on servers using Node.js.

**💻 Example:**

```javascript
console.log("Hello, JavaScript!");
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q2. What are the main data types in JavaScript?

**✅ Easy Explanation:** JavaScript has seven primitive types: string, number, bigint, boolean, undefined, symbol, and null. Objects are non-primitive.

**💻 Example:**

```javascript
const name = "Asha";
const age = 25;
const active = true;
const user = { name, age };
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q3. What is the difference between `var`, `let`, and `const`?

**✅ Easy Explanation:** `var` is function-scoped and can be redeclared. `let` and `const` are block-scoped. `let` can be reassigned, but `const` cannot be reassigned.

**💻 Example:**

```javascript
let count = 1;
count = 2;
const city = "Delhi";
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q4. What is hoisting?

**✅ Easy Explanation:** Hoisting means declarations are processed before code executes. `var` starts as `undefined`; `let` and `const` stay in the temporal dead zone until their declaration runs.

**💻 Example:**

```javascript
console.log(a); // undefined
var a = 10;
// console.log(b); // ReferenceError
let b = 20;
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q5. What is the temporal dead zone (TDZ)?

**✅ Easy Explanation:** TDZ is the time from entering a block until a `let` or `const` declaration executes. Accessing the variable during this period throws `ReferenceError`.

**💻 Example:**

```javascript
{
  // console.log(score); // ReferenceError
  const score = 90;
  console.log(score);
}
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q6. What is the difference between `==` and `===`?

**✅ Easy Explanation:** `==` may convert values before comparing. `===` compares without type conversion. Prefer `===` to avoid confusing results.

**💻 Example:**

```javascript
console.log(5 == "5");  // true
console.log(5 === "5"); // false
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q7. What are truthy and falsy values?

**✅ Easy Explanation:** Falsy values include `false`, `0`, `-0`, `0n`, `""`, `null`, `undefined`, and `NaN`. Other values, including `[]` and `{}`, are truthy.

**💻 Example:**

```javascript
console.log(Boolean("")); // false
console.log(Boolean([])); // true
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q8. What is the difference between `null` and `undefined`?

**✅ Easy Explanation:** `undefined` usually means no value was assigned. `null` is an intentional empty value. Both are different types of absence.

**💻 Example:**

```javascript
let result;
const selectedUser = null;
console.log(result, selectedUser);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q9. What is `NaN`?

**✅ Easy Explanation:** `NaN` means Not-a-Number. It is a special numeric value for an invalid number result. Use `Number.isNaN()` to check it.

**💻 Example:**

```javascript
const value = Number("abc");
console.log(Number.isNaN(value)); // true
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q10. What does `typeof` do?

**✅ Easy Explanation:** `typeof` returns a string describing a value type. One old JavaScript quirk is that `typeof null` returns `"object"`.

**💻 Example:**

```javascript
console.log(typeof 42); // number
console.log(typeof null); // object
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q11. What is type coercion?

**✅ Easy Explanation:** Type coercion means JavaScript converts a value from one type to another when an operation needs it. Explicit conversion is easier to read.

**💻 Example:**

```javascript
console.log("5" + 2); // "52"
console.log("5" - 2); // 3
console.log(Number("5") + 2); // 7
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q12. What is the difference between primitive and reference values?

**✅ Easy Explanation:** Primitive values are copied as values. Objects are copied as references to the same object, so a change through one reference is visible through the other.

**💻 Example:**

```javascript
let a = 5;
let b = a; b = 9;
const x = { n: 1 };
const y = x; y.n = 2;
console.log(a, x.n); // 5 2
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q13. What is a template literal?

**✅ Easy Explanation:** Template literals use backticks. They support `${...}` interpolation and multi-line text, so building readable strings becomes simple.

**💻 Example:**

```javascript
const name = "Ravi";
console.log(`Welcome, ${name}!`);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q14. What is destructuring?

**✅ Easy Explanation:** Destructuring extracts values from arrays or properties from objects into variables in one simple step.

**💻 Example:**

```javascript
const [first, second] = [10, 20];
const { name } = { name: "Neha", age: 24 };
console.log(first, second, name);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q15. What is the spread operator (`...`)?

**✅ Easy Explanation:** Spread expands array elements or object properties. It is useful for copying and merging, but nested objects still share references.

**💻 Example:**

```javascript
const nums = [1, 2];
const more = [...nums, 3];
const user = { name: "Ali" };
const updated = { ...user, active: true };
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q16. What is the rest parameter (`...`)?

**✅ Easy Explanation:** Rest collects remaining function arguments into an array. Unlike the old `arguments` object, it is a real array.

**💻 Example:**

```javascript
function add(...numbers) {
  return numbers.reduce((sum, n) => sum + n, 0);
}
console.log(add(1, 2, 3)); // 6
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q17. What is optional chaining (`?.`)?

**✅ Easy Explanation:** Optional chaining safely reads a nested property or calls a method when the value before `?.` may be `null` or `undefined`.

**💻 Example:**

```javascript
const user = {};
console.log(user.address?.city); // undefined
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q18. What is nullish coalescing (`??`)?

**✅ Easy Explanation:** `??` uses a fallback only when the left side is `null` or `undefined`. It keeps valid values like `0`, `false`, and an empty string.

**💻 Example:**

```javascript
const quantity = 0;
console.log(quantity ?? 10); // 0
console.log(quantity || 10); // 10
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

</details>


<a id="section-2"></a>
## 2. Functions, Scope & Closures

<details open>
<summary><strong>Expand / collapse questions</strong></summary>

### Q19. What is a function declaration?

**✅ Easy Explanation:** A function declaration defines a named reusable function. It can generally be called before its declaration in the same scope.

**💻 Example:**

```javascript
console.log(square(4)); // 16
function square(n) { return n * n; }
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q20. What is a function expression?

**✅ Easy Explanation:** A function expression stores a function in a variable. You can call it after the variable has been initialised.

**💻 Example:**

```javascript
const greet = function(name) {
  return `Hi, ${name}`;
};
console.log(greet("Anu"));
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q21. What is an arrow function?

**✅ Easy Explanation:** An arrow function is concise and takes `this` from its surrounding scope. It does not have its own `arguments` and cannot be used as a constructor.

**💻 Example:**

```javascript
const double = n => n * 2;
console.log(double(6)); // 12
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q22. How are arrow functions different from regular functions?

**✅ Easy Explanation:** Regular functions usually get `this` from how they are called. Arrows capture the surrounding `this`, so arrows are good for callbacks but often unsuitable as object methods.

**💻 Example:**

```javascript
const counter = {
  count: 2,
  getCount() { return this.count; }
};
console.log(counter.getCount()); // 2
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q23. What is lexical scope?

**✅ Easy Explanation:** Lexical scope means a function can access variables from the place where the function was written, including its outer functions.

**💻 Example:**

```javascript
const city = "Pune";
function showCity() { console.log(city); }
showCity();
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q24. What is a closure?

**✅ Easy Explanation:** A closure is a function that remembers variables from its outer scope even after that outer function has returned. Useful for private state.

**💻 Example:**

```javascript
function makeCounter() {
  let count = 0;
  return () => ++count;
}
const next = makeCounter();
console.log(next(), next()); // 1 2
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q25. What is a callback function?

**✅ Easy Explanation:** A callback is a function passed to another function to execute later or at a chosen point. It may be synchronous or asynchronous.

**💻 Example:**

```javascript
function process(value, callback) {
  return callback(value);
}
console.log(process(4, n => n * 2)); // 8
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q26. What is a higher-order function?

**✅ Easy Explanation:** A higher-order function takes a function as an argument or returns a function. Examples include `map`, `filter`, and `reduce`.

**💻 Example:**

```javascript
const values = [1, 2, 3];
const doubled = values.map(n => n * 2);
console.log(doubled); // [2, 4, 6]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q27. What is an IIFE?

**✅ Easy Explanation:** IIFE stands for Immediately Invoked Function Expression. It runs as soon as it is created and can keep temporary variables private.

**💻 Example:**

```javascript
(() => {
  const message = "Ready";
  console.log(message);
})();
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q28. What is recursion?

**✅ Easy Explanation:** Recursion is when a function calls itself. Always write a stopping condition, otherwise it may keep calling until the call stack overflows.

**💻 Example:**

```javascript
function factorial(n) {
  if (n <= 1) return 1;
  return n * factorial(n - 1);
}
console.log(factorial(5)); // 120
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q29. What are default parameters?

**✅ Easy Explanation:** Default parameters give function arguments a fallback when the passed value is `undefined` or when no value is passed.

**💻 Example:**

```javascript
function greet(name = "Guest") {
  return `Hello ${name}`;
}
console.log(greet()); // Hello Guest
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q30. What is currying?

**✅ Easy Explanation:** Currying changes a function taking multiple arguments into a chain of functions taking one argument at a time. It helps to create reusable configured functions.

**💻 Example:**

```javascript
const multiply = a => b => a * b;
const double = multiply(2);
console.log(double(7)); // 14
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q31. What is a pure function?

**✅ Easy Explanation:** A pure function returns the same output for the same inputs and does not change outside state. Pure functions are easier to test.

**💻 Example:**

```javascript
function add(a, b) { return a + b; }
console.log(add(2, 3)); // 5
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q32. What is memoization?

**✅ Easy Explanation:** Memoization stores the result of a previous calculation and reuses it when the same input comes again. It saves repeated work.

**💻 Example:**

```javascript
const cache = new Map();
function square(n) {
  if (cache.has(n)) return cache.get(n);
  const answer = n * n;
  cache.set(n, answer);
  return answer;
}
console.log(square(5)); // 25
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q33. What does `this` mean in JavaScript?

**✅ Easy Explanation:** `this` refers to the context of a call. For a normal object method, it is usually the object before the dot; arrows inherit `this` lexically.

**💻 Example:**

```javascript
const user = {
  name: "Sara",
  sayName() { return this.name; }
};
console.log(user.sayName()); // Sara
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q34. What is the difference between `call`, `apply`, and `bind`?

**✅ Easy Explanation:** All three can set `this` for a regular function. `call` takes individual arguments, `apply` takes an array-like list, and `bind` returns a new function.

**💻 Example:**

```javascript
function hello(greeting) { return `${greeting}, ${this.name}`; }
const person = { name: "Amit" };
console.log(hello.call(person, "Hi"));
console.log(hello.apply(person, ["Hello"]));
console.log(hello.bind(person)("Hey"));
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q35. What is debouncing?

**✅ Easy Explanation:** Debouncing waits until repeated activity stops for a given time, then runs the function once. Useful for a search box.

**💻 Example:**

```javascript
function debounce(fn, delay) {
  let timer;
  return (...args) => {
    clearTimeout(timer);
    timer = setTimeout(() => fn(...args), delay);
  };
}
const search = debounce(query => console.log(query), 300);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q36. What is throttling?

**✅ Easy Explanation:** Throttling limits how often a function can run during repeated events. Useful for scroll or resize handlers.

**💻 Example:**

```javascript
function throttle(fn, delay) {
  let last = 0;
  return (...args) => {
    const now = Date.now();
    if (now - last >= delay) {
      last = now;
      fn(...args);
    }
  };
}
const onScroll = throttle(() => console.log("scroll"), 200);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

</details>


<a id="section-3"></a>
## 3. Arrays, Strings & Objects

<details open>
<summary><strong>Expand / collapse questions</strong></summary>

### Q37. What is the difference between `map()` and `forEach()`?

**✅ Easy Explanation:** `map()` creates a new array from returned values. `forEach()` runs code for each item and returns `undefined`.

**💻 Example:**

```javascript
const nums = [1, 2, 3];
console.log(nums.map(n => n * 2)); // [2, 4, 6]
nums.forEach(n => console.log(n));
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q38. How does `filter()` work?

**✅ Easy Explanation:** `filter()` returns a new array containing only items for which the callback gives a truthy result.

**💻 Example:**

```javascript
const ages = [16, 21, 18, 14];
console.log(ages.filter(age => age >= 18)); // [21, 18]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q39. How does `reduce()` work?

**✅ Easy Explanation:** `reduce()` combines array items into one accumulated result. The initial value is important, especially for empty arrays.

**💻 Example:**

```javascript
const total = [10, 20, 30].reduce((sum, n) => sum + n, 0);
console.log(total); // 60
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q40. What is the difference between `find()` and `filter()`?

**✅ Easy Explanation:** `find()` returns the first matching item or `undefined`. `filter()` returns all matching items in an array.

**💻 Example:**

```javascript
const nums = [2, 3, 4, 5];
console.log(nums.find(n => n > 3)); // 4
console.log(nums.filter(n => n > 3)); // [4, 5]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q41. What is the difference between `slice()` and `splice()`?

**✅ Easy Explanation:** `slice()` returns a selected part without changing the original array. `splice()` changes the array by removing or inserting elements.

**💻 Example:**

```javascript
const a = [1, 2, 3, 4];
console.log(a.slice(1, 3)); // [2, 3]
a.splice(1, 1);
console.log(a); // [1, 3, 4]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q42. How does `sort()` work?

**✅ Easy Explanation:** By default, `sort()` compares items as strings and changes the original array. Provide a comparator for numeric sorting.

**💻 Example:**

```javascript
const nums = [10, 2, 30];
nums.sort((a, b) => a - b);
console.log(nums); // [2, 10, 30]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q43. How do you remove duplicates from an array?

**✅ Easy Explanation:** A `Set` stores unique values. Convert the set back into an array using spread. Objects are compared by reference, not their content.

**💻 Example:**

```javascript
const values = [1, 2, 2, 3, 1];
const unique = [...new Set(values)];
console.log(unique); // [1, 2, 3]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q44. How do you flatten a nested array?

**✅ Easy Explanation:** Use `flat(depth)` to combine nested array levels. `Infinity` flattens all nested levels.

**💻 Example:**

```javascript
const data = [1, [2, [3, 4]]];
console.log(data.flat(Infinity)); // [1, 2, 3, 4]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q45. How do you check whether a value is an array?

**✅ Easy Explanation:** Use `Array.isArray()` because `typeof []` returns `"object"`, which is not specific enough.

**💻 Example:**

```javascript
console.log(Array.isArray([1, 2])); // true
console.log(Array.isArray({ 0: 1 })); // false
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q46. How do you reverse a string?

**✅ Easy Explanation:** Convert the string into characters, reverse them, and join again. This simple approach works for common text, but not every combined Unicode grapheme.

**💻 Example:**

```javascript
function reverseText(text) {
  return [...text].reverse().join("");
}
console.log(reverseText("hello")); // olleh
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q47. How do you check whether a string is a palindrome?

**✅ Easy Explanation:** A palindrome reads the same forwards and backwards. Normalise case and remove non-alphanumeric characters if your problem allows it.

**💻 Example:**

```javascript
function isPalindrome(text) {
  const clean = text.toLowerCase().replace(/[^a-z0-9]/g, "");
  return clean === [...clean].reverse().join("");
}
console.log(isPalindrome("Madam")); // true
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q48. How do you count character frequency?

**✅ Easy Explanation:** Loop through the characters and store each character count in a `Map` or object.

**💻 Example:**

```javascript
const counts = new Map();
for (const char of "banana") {
  counts.set(char, (counts.get(char) ?? 0) + 1);
}
console.log(counts.get("a")); // 3
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q49. What is the difference between `Object.keys()`, `Object.values()`, and `Object.entries()`?

**✅ Easy Explanation:** `keys()` gives property names, `values()` gives property values, and `entries()` gives `[key, value]` pairs of own enumerable string-keyed properties.

**💻 Example:**

```javascript
const user = { name: "Isha", age: 22 };
console.log(Object.keys(user));
console.log(Object.values(user));
console.log(Object.entries(user));
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q50. How do you merge two objects?

**✅ Easy Explanation:** Use object spread or `Object.assign()`. Later properties override earlier ones. Both approaches make a shallow copy.

**💻 Example:**

```javascript
const a = { x: 1, y: 2 };
const b = { y: 5, z: 6 };
console.log({ ...a, ...b }); // {x:1,y:5,z:6}
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q51. What is shallow copy vs deep copy?

**✅ Easy Explanation:** A shallow copy duplicates only the outer container, while nested objects remain shared. A deep copy copies nested structures too.

**💻 Example:**

```javascript
const original = { profile: { age: 20 } };
const shallow = { ...original };
const deep = structuredClone(original);
shallow.profile.age = 21;
console.log(original.profile.age); // 21
console.log(deep.profile.age); // 20
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q52. What does `Object.freeze()` do?

**✅ Easy Explanation:** `Object.freeze()` prevents adding, deleting, or changing own properties of that object. It is shallow, so nested objects can still change unless frozen too.

**💻 Example:**

```javascript
const config = Object.freeze({ mode: "dark" });
console.log(config.mode); // dark
console.log(Object.isFrozen(config)); // true
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q53. What is the difference between `Map` and a plain object?

**✅ Easy Explanation:** `Map` accepts keys of any type and offers `set`, `get`, and `has`. Objects are useful for structured records with string or symbol property keys.

**💻 Example:**

```javascript
const map = new Map();
const key = { id: 1 };
map.set(key, "value");
console.log(map.get(key)); // value
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q54. What is a `Set`?

**✅ Easy Explanation:** A `Set` holds unique values. It is useful for removing duplicates and fast membership checks.

**💻 Example:**

```javascript
const skills = new Set(["JS", "React", "JS"]);
console.log(skills.size); // 2
console.log(skills.has("React")); // true
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

</details>


<a id="section-4"></a>
## 4. Asynchronous JavaScript & Event Loop

<details open>
<summary><strong>Expand / collapse questions</strong></summary>

### Q55. What is synchronous vs asynchronous JavaScript?

**✅ Easy Explanation:** Synchronous code runs in sequence. Asynchronous operations can complete later without blocking the current JavaScript task, for example timers or network requests.

**💻 Example:**

```javascript
console.log("A");
setTimeout(() => console.log("C"), 0);
console.log("B"); // A, B, C
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q56. What is the call stack?

**✅ Easy Explanation:** The call stack tracks currently running function calls. A function is pushed when called and removed when it returns.

**💻 Example:**

```javascript
function first() { second(); }
function second() { console.log("Done"); }
first();
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q57. What is the event loop?

**✅ Easy Explanation:** The event loop coordinates JavaScript execution with queued jobs. Once the current stack is empty, queued microtasks run before the next timer task in normal browser execution.

**💻 Example:**

```javascript
console.log("1");
setTimeout(() => console.log("3"), 0);
Promise.resolve().then(() => console.log("2"));
// 1, 2, 3
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q58. What is the difference between microtasks and macrotasks?

**✅ Easy Explanation:** Promise reactions and `queueMicrotask` use the microtask queue. Timers use task queues. Microtasks are drained before the event loop moves to another task.

**💻 Example:**

```javascript
setTimeout(() => console.log("timer"), 0);
queueMicrotask(() => console.log("microtask"));
// microtask, timer
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q59. What is a Promise?

**✅ Easy Explanation:** A Promise represents an asynchronous result that is pending, fulfilled, or rejected. `.then()` handles success and `.catch()` handles failure.

**💻 Example:**

```javascript
const promise = Promise.resolve("Success");
promise.then(value => console.log(value));
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q60. What is Promise chaining?

**✅ Easy Explanation:** Returning a value or Promise from `.then()` passes the result to the next `.then()`. Return each asynchronous step instead of nesting unnecessarily.

**💻 Example:**

```javascript
Promise.resolve(2)
  .then(n => n * 3)
  .then(n => console.log(n)) // 6
  .catch(console.error);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q61. What is `async/await`?

**✅ Easy Explanation:** An `async` function returns a Promise. `await` pauses that function until a Promise settles, making asynchronous code look easier to read.

**💻 Example:**

```javascript
async function getNumber() {
  const value = await Promise.resolve(42);
  return value;
}
getNumber().then(console.log);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q62. How do you handle errors with `async/await`?

**✅ Easy Explanation:** Use `try/catch` around awaited work. Catch the error and show or log a useful message instead of silently ignoring it.

**💻 Example:**

```javascript
async function load() {
  try {
    const result = await Promise.reject(new Error("Failed"));
    return result;
  } catch (error) {
    console.log(error.message);
  }
}
load();
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q63. What is `Promise.all()`?

**✅ Easy Explanation:** `Promise.all()` waits for all supplied promises to fulfil. It rejects as soon as any input rejects; it does not cancel the other operations.

**💻 Example:**

```javascript
Promise.all([Promise.resolve(2), Promise.resolve(4)])
  .then(values => console.log(values)); // [2, 4]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q64. What is `Promise.allSettled()`?

**✅ Easy Explanation:** `Promise.allSettled()` waits for every Promise and returns objects showing whether each fulfilled or rejected. Useful when one failure should not hide other results.

**💻 Example:**

```javascript
Promise.allSettled([Promise.resolve(1), Promise.reject("Oops")])
  .then(results => console.log(results.map(r => r.status)));
// ["fulfilled", "rejected"]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q65. What is `Promise.race()`?

**✅ Easy Explanation:** `Promise.race()` settles with the outcome of the first input Promise that settles, whether it fulfils or rejects.

**💻 Example:**

```javascript
Promise.race([
  Promise.resolve("fast"),
  new Promise(resolve => setTimeout(() => resolve("slow"), 100))
]).then(console.log); // fast
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q66. What is `Promise.any()`?

**✅ Easy Explanation:** `Promise.any()` fulfils with the first fulfilled result. It rejects with an `AggregateError` only if all inputs reject.

**💻 Example:**

```javascript
Promise.any([Promise.reject("No"), Promise.resolve("Yes")])
  .then(console.log); // Yes
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q67. What is callback hell?

**✅ Easy Explanation:** Callback hell happens when many nested callbacks make code hard to follow and errors hard to manage. Promises and async/await help flatten the flow.

**💻 Example:**

```javascript
async function runSteps() {
  const a = await Promise.resolve(1);
  const b = await Promise.resolve(a + 1);
  console.log(b);
}
runSteps();
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q68. What does `setTimeout(fn, 0)` really mean?

**✅ Easy Explanation:** It schedules a callback to run after at least the timer delay, not immediately. Current synchronous code and pending microtasks finish first.

**💻 Example:**

```javascript
setTimeout(() => console.log("Later"), 0);
console.log("Now"); // Now, Later
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q69. How do you use `fetch()` to call an API?

**✅ Easy Explanation:** `fetch()` returns a Promise for a `Response`. Check `response.ok` for HTTP errors, then parse the body with `.json()` or another body method.

**💻 Example:**

```javascript
async function getUser() {
  const response = await fetch("https://jsonplaceholder.typicode.com/users/1");
  if (!response.ok) throw new Error(`HTTP ${response.status}`);
  return response.json();
}
getUser().then(console.log).catch(console.error);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q70. How do you cancel a `fetch()` request?

**✅ Easy Explanation:** Create an `AbortController`, pass its `signal` to `fetch()`, then call `abort()` when the request is no longer needed.

**💻 Example:**

```javascript
const controller = new AbortController();
fetch("https://example.com/data", { signal: controller.signal })
  .catch(error => {
    if (error.name !== "AbortError") console.error(error);
  });
controller.abort();
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q71. How can you run async operations concurrently?

**✅ Easy Explanation:** Start independent operations together and await them using `Promise.all()` instead of awaiting each one one-by-one.

**💻 Example:**

```javascript
async function loadBoth() {
  const [a, b] = await Promise.all([
    Promise.resolve("users"),
    Promise.resolve("posts")
  ]);
  console.log(a, b);
}
loadBoth();
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q72. How do you retry a failed async operation?

**✅ Easy Explanation:** Wrap the operation in a loop, catching failures and trying again up to a limit. In production, consider delays and only retry safe operations.

**💻 Example:**

```javascript
async function retry(fn, attempts = 3) {
  for (let i = 1; i <= attempts; i++) {
    try { return await fn(); }
    catch (error) { if (i === attempts) throw error; }
  }
}
retry(() => Promise.resolve("OK")).then(console.log);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

</details>


<a id="section-5"></a>
## 5. DOM, Browser & Events

<details open>
<summary><strong>Expand / collapse questions</strong></summary>

### Q73. What is the DOM?

**✅ Easy Explanation:** The Document Object Model represents an HTML document as objects. JavaScript can read, change, add, or remove elements using DOM APIs.

**💻 Example:**

```javascript
// Run in a browser with an element having id="title"
const heading = document.getElementById("title");
if (heading) heading.textContent = "Hello DOM";
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q74. What is the difference between `querySelector()` and `querySelectorAll()`?

**✅ Easy Explanation:** `querySelector()` returns the first matching element or `null`. `querySelectorAll()` returns a static NodeList of all matches.

**💻 Example:**

```javascript
const firstButton = document.querySelector("button");
const allButtons = document.querySelectorAll("button");
console.log(allButtons.length);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q75. What is event bubbling?

**✅ Easy Explanation:** In bubbling, an event usually travels from the target element up through its ancestors. You can respond on a parent to child events.

**💻 Example:**

```javascript
document.body.addEventListener("click", event => {
  console.log("Clicked:", event.target.tagName);
});
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q76. What is event delegation?

**✅ Easy Explanation:** Event delegation puts one listener on a parent and checks which child caused the event. It also works for matching children added later.

**💻 Example:**

```javascript
document.addEventListener("click", event => {
  const button = event.target.closest("[data-action]");
  if (button) console.log(button.dataset.action);
});
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q77. What is the difference between `preventDefault()` and `stopPropagation()`?

**✅ Easy Explanation:** `preventDefault()` cancels a cancelable browser default action. `stopPropagation()` stops the event from moving to other elements in the propagation path.

**💻 Example:**

```javascript
document.addEventListener("submit", event => {
  event.preventDefault(); // avoid normal form submission
});
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q78. What is the difference between `innerHTML` and `textContent`?

**✅ Easy Explanation:** `textContent` treats text as plain text. `innerHTML` parses HTML markup; do not insert untrusted input into it because this can cause XSS.

**💻 Example:**

```javascript
const el = document.createElement("div");
el.textContent = "<strong>Safe text</strong>";
console.log(el.textContent);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q79. What is localStorage vs sessionStorage?

**✅ Easy Explanation:** Both store string key-value pairs per origin. `localStorage` usually persists across browser sessions; `sessionStorage` is scoped to a page session/tab.

**💻 Example:**

```javascript
localStorage.setItem("theme", "dark");
console.log(localStorage.getItem("theme"));
sessionStorage.setItem("step", "2");
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q80. What are cookies?

**✅ Easy Explanation:** Cookies are small values stored by the browser and may be sent with HTTP requests. Server-set cookies can use flags like `HttpOnly`, `Secure`, and `SameSite`.

**💻 Example:**

```javascript
// Browser example (not HttpOnly):
document.cookie = "language=en; Path=/; SameSite=Lax";
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q81. What is CORS?

**✅ Easy Explanation:** Cross-Origin Resource Sharing is a browser security mechanism. A server uses response headers to allow approved cross-origin requests; frontend JavaScript cannot simply disable it.

**💻 Example:**

```javascript
// Server must allow your origin when needed.
fetch("https://api.example.com/data")
  .then(response => console.log(response.status))
  .catch(console.error);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

</details>


<a id="section-6"></a>
## 6. Objects, Prototypes & Advanced Concepts

<details open>
<summary><strong>Expand / collapse questions</strong></summary>

### Q82. What is prototypal inheritance?

**✅ Easy Explanation:** JavaScript objects can inherit properties and methods through a prototype chain. If a property is not on an object, lookup can continue on its prototype.

**💻 Example:**

```javascript
const parent = { greet() { return "Hello"; } };
const child = Object.create(parent);
console.log(child.greet()); // Hello
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q83. What is the difference between `prototype` and `__proto__`?

**✅ Easy Explanation:** A constructor function’s `prototype` is used for instances created with `new`. `__proto__` is a legacy accessor for an object’s prototype; prefer `Object.getPrototypeOf()`.

**💻 Example:**

```javascript
function Person(name) { this.name = name; }
const user = new Person("Riya");
console.log(Object.getPrototypeOf(user) === Person.prototype); // true
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q84. What does the `new` keyword do?

**✅ Easy Explanation:** `new` creates an object, links it to the constructor’s `prototype`, runs the constructor with that object as `this`, and usually returns the object.

**💻 Example:**

```javascript
function User(name) { this.name = name; }
const user = new User("Kabir");
console.log(user.name); // Kabir
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q85. What are JavaScript classes?

**✅ Easy Explanation:** A class provides cleaner syntax for constructors and prototype methods. Under the hood, JavaScript still uses prototype-based inheritance.

**💻 Example:**

```javascript
class User {
  constructor(name) { this.name = name; }
  greet() { return `Hi ${this.name}`; }
}
console.log(new User("Maya").greet());
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q86. What are private class fields?

**✅ Easy Explanation:** Fields starting with `#` are accessible only inside the class body. They help keep internal state private.

**💻 Example:**

```javascript
class Counter {
  #count = 0;
  increment() { return ++this.#count; }
}
console.log(new Counter().increment()); // 1
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q87. What are JavaScript modules?

**✅ Easy Explanation:** Modules allow files to export and import reusable functions or values. Modern ES modules use `export` and `import` and are automatically in strict mode.

**💻 Example:**

```javascript
// math.js
export const add = (a, b) => a + b;
// app.js
// import { add } from "./math.js";
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q88. What is the difference between named and default exports?

**✅ Easy Explanation:** Named exports are imported with matching names (or aliases). A module can have one default export, imported with a chosen local name.

**💻 Example:**

```javascript
// utils.js
export const version = "1.0";
export default function greet() { return "Hi"; }
// import greet, { version } from "./utils.js";
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q89. What is a generator function?

**✅ Easy Explanation:** A generator uses `function*` and `yield` to produce values one at a time. Calling it gives an iterator rather than executing everything immediately.

**💻 Example:**

```javascript
function* numbers() {
  yield 1;
  yield 2;
}
console.log([...numbers()]); // [1, 2]
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q90. What is the difference between `for...in` and `for...of`?

**✅ Easy Explanation:** `for...in` loops through enumerable string property keys (including inherited keys). `for...of` loops over values from an iterable such as an array or string.

**💻 Example:**

```javascript
const items = ["a", "b"];
for (const index in items) console.log(index); // "0", "1"
for (const value of items) console.log(value); // a, b
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q91. What is garbage collection in JavaScript?

**✅ Easy Explanation:** Garbage collection automatically reclaims memory for objects that are no longer reachable from live references. You still need to avoid keeping unnecessary references.

**💻 Example:**

```javascript
let data = { items: [1, 2, 3] };
data = null; // original object may become collectible
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q92. What causes memory leaks in JavaScript?

**✅ Easy Explanation:** Leaks often come from unused timers, event listeners, or caches that keep references alive. Remove listeners and clear timers when they are no longer needed.

**💻 Example:**

```javascript
const timer = setInterval(() => console.log("tick"), 1000);
clearInterval(timer); // cleanup
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q93. What is a `WeakMap`?

**✅ Easy Explanation:** A `WeakMap` accepts objects and non-registered symbols as keys and does not keep its object keys alive by itself. Useful for metadata without retaining objects unnecessarily.

**💻 Example:**

```javascript
const privateInfo = new WeakMap();
const user = {};
privateInfo.set(user, { token: "hidden" });
console.log(privateInfo.get(user).token);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q94. What is `JSON.stringify()` vs `JSON.parse()`?

**✅ Easy Explanation:** `JSON.stringify()` converts supported JavaScript data into a JSON string. `JSON.parse()` reads a JSON string into a JavaScript value. JSON does not preserve functions or `undefined` object properties.

**💻 Example:**

```javascript
const text = JSON.stringify({ name: "Dev", age: 26 });
const user = JSON.parse(text);
console.log(user.name); // Dev
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q95. What is the difference between `Object.is()` and `===`?

**✅ Easy Explanation:** They are mostly similar, but `Object.is(NaN, NaN)` is true and `Object.is(0, -0)` is false. With `===`, those results are reversed.

**💻 Example:**

```javascript
console.log(Object.is(NaN, NaN)); // true
console.log(NaN === NaN); // false
console.log(Object.is(0, -0)); // false
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q96. What is a `Symbol`?

**✅ Easy Explanation:** A Symbol is a unique primitive value often used as an object property key to avoid accidental name collisions.

**💻 Example:**

```javascript
const id = Symbol("id");
const user = { [id]: 123 };
console.log(user[id]); // 123
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q97. What is `BigInt`?

**✅ Easy Explanation:** `BigInt` represents integers beyond the safe integer range of Number. Add `n` to integer literals and do not directly mix BigInt and Number arithmetic.

**💻 Example:**

```javascript
const big = 9007199254740993n;
console.log(big + 1n); // 9007199254740994n
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q98. How does optional error handling with `try/catch/finally` work?

**✅ Easy Explanation:** `try` runs risky code, `catch` handles thrown errors, and `finally` runs cleanup code whether an error happened or not.

**💻 Example:**

```javascript
try {
  JSON.parse("not-json");
} catch (error) {
  console.log("Invalid JSON");
} finally {
  console.log("Finished");
}
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q99. What is XSS and how can JavaScript prevent it?

**✅ Easy Explanation:** Cross-site scripting happens when attacker-controlled content runs as script in a page. Use `textContent`, safe templating, and proper sanitisation for trusted HTML workflows.

**💻 Example:**

```javascript
const message = "<img src=x onerror=alert(1)>";
const element = document.createElement("p");
element.textContent = message; // displays text, not HTML
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

### Q100. How do you improve JavaScript performance?

**✅ Easy Explanation:** Measure before optimising. Avoid unnecessary DOM work, debounce frequent events, cache costly computations when useful, and keep long work off the main thread where possible.

**💻 Example:**

```javascript
const list = document.createDocumentFragment();
for (let i = 0; i < 3; i++) {
  const item = document.createElement("li");
  item.textContent = `Item ${i}`;
  list.appendChild(item);
}
// document.querySelector("ul")?.appendChild(list);
```

<sub>↩️ [Back to top](#-javascript-interview-questions--answers)</sub>

---

</details>


## 🎯 Interview Preparation Tips

1. First understand the concept; do not just memorise the answer.
2. Run every code example and try changing the input.
3. Practise explaining the output without looking at the notes.
4. Revise closures, `this`, promises, the event loop, and array methods regularly.
5. Build a small JavaScript project to apply these concepts.

## ▶️ How to Run the Examples

1. Install a recent Node.js LTS version for general JavaScript examples.
2. Save any standalone example in `practice.js`, then run `node practice.js`.
3. For DOM, `localStorage`, cookies, or browser-specific `fetch` examples, use browser DevTools on a suitable webpage.
4. Some examples are educational snippets (for example, module imports across two files) and need the surrounding setup shown in comments.

## 🤝 Contributing

Found a mistake or have a clearer example? Contributions and pull requests are welcome. Keep answers accurate, easy to understand, and beginner-friendly.

## ⭐ Support

If this guide helps with your interview preparation, please **star ⭐ this repository** and share it with another developer.

---

<div align="center">

**Happy Coding! 💛**

</div>
