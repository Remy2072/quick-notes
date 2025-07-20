# JavaScript Cheat Sheet

## Variables

-   `let`: variable that can be reassigned.
-   `const`: variable that cannot be reassigned.
-   `var`: outdated, avoid using it.

### Examples

```javascript
let username;
username = "Remy";
username = "Mike"; // ✅ Valid

const name = "Remy";
name = "Mike"; // ❌ Error
```

---

## Naming Rules

-   Must start with a letter, `_` or `$`.
-   Cannot contain spaces.
-   Avoid reserved keywords like `let`, `class`, `return`, etc.

### Valid Examples

```javascript
let a;
let color;
let _private;
let $button;
let getTop10;
let a_large_name;
let camelCase;
```

---

## Data Types

### Primitive Types

-   String
-   Number
-   Boolean
-   Undefined
-   Null

```javascript
let name = "abc123.?!$"; // string
let age = 22; // number
let isLoggedIn = false; // boolean
```

### Reference Types

-   Object
-   Array

---

## Arithmetic Operators

```javascript
let a = 10;
let b = 5;

console.log(a + b); // Addition
console.log(a - b); // Subtraction
console.log(a * b); // Multiplication
console.log(a / b); // Division
console.log(a % b); // Modulo (remainder)
console.log(4 ** 3); // Exponentiation

let age = 22;
age += 1; // 23
age++; // 24
```

---

## Comparison Operators

```javascript
let x = 5;

console.log(x > 7); // false
console.log(x < 7); // true
console.log(x == 5); // true (loose equality)
console.log(6 >= 5); // true
console.log(4 <= 5); // true
console.log(10 != 5); // true
console.log(10 != 10); // false

console.log(5 == "5"); // true (type coercion)
console.log(5 === "5"); // false (strict comparison)
console.log(false == 0); // true
console.log(undefined == null); // true
console.log("" == 0); // true
console.log("6" !== 6); // true
```

---

## If Statements

```javascript
let dbPassword = "1234";
let enteredPassword = "1234";
let enteredUsername = "Remy";

if (enteredPassword === dbPassword) {
    console.log("Welcome " + enteredUsername);
} else {
    console.log("Wrong password");
}
```

```javascript
let language = "spanish";

if (language === "spanish") {
    console.log("Bienvenido!");
} else if (language === "german") {
    console.log("Moin! Moin! Moin!");
} else if (language === "english") {
    console.log("Welcome!");
} else {
    console.log("We don't support: " + language);
}
```

---

## Loops

### While Loop

```javascript
let counter = 0;

while (counter < 10) {
    console.log(counter);
    counter++;
}
```

### For Loop

```javascript
for (let i = 0; i < 10; i++) {
    console.log(i);
}
```

---

## Functions

### No Parameters

```javascript
function sayHello() {
    console.log("Hello World");
}

sayHello();
```

### With One Parameter

```javascript
function sayHello(name) {
    console.log("Hello " + name);
}

sayHello("Remy");
```

### With Multiple Parameters

```javascript
function addNumbers(num1, num2) {
    console.log(num1 + num2);
}

addNumbers(5, 3); // 8
```

---

## DOM (Document Object Model)

> Use the `defer` attribute in your `<script>` tag to ensure the DOM is loaded before running scripts.

### Injecting HTML

```javascript
document.body.innerHTML = "<h1>Hello World</h1>";
document.body.innerHTML += "<button>Click me</button>";
```

### Changing Styles

```javascript
document.body.style.color = "blue";
document.body.style.backgroundColor = "lightgray";
```
