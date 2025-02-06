

```markdown
# JavaScript Loops and Switch-Case Explanation

This guide explains the different types of loops in JavaScript: `for`, `while`, `do...while`, and `switch-case` statements. Each section provides a detailed explanation, when to use them, and five examples of how to use them with normal variables.

## 1. `for` Loop

The `for` loop is used when you know the number of iterations in advance. It is commonly used to repeat a block of code a set number of times.

### Syntax:
```javascript
for (initialization; condition; increment/decrement) {
    // code block to be executed
}
```

### When to Use:
- When you know how many times you need to repeat something.
- Example: Looping through numbers 1 to 5.

### Examples:

1. **Basic `for` loop from 1 to 5:**
```javascript
for (let i = 1; i <= 5; i++) {
    console.log(i);  // Output: 1 2 3 4 5
}
```

2. **Sum of numbers 1 to 10:**
```javascript
let result = 0;
for (let i = 1; i <= 10; i++) {
    result += i;  // Adds numbers 1 to 10
}
console.log(result);  // Output: 55
```

3. **Incrementing counter by 2:**
```javascript
let counter = 0;
for (let i = 0; i < 10; i++) {
    counter += 2;
}
console.log(counter);  // Output: 20
```

4. **Countdown from 10 to 1:**
```javascript
for (let i = 10; i >= 1; i--) {
    console.log(i);  // Output: 10 9 8 7 6 5 4 3 2 1
}
```

5. **Sum of squares of numbers 1 to 5:**
```javascript
let sum = 0;
for (let i = 1; i <= 5; i++) {
    sum = sum + i * i;  // Adding the square of each number
}
console.log(sum);  // Output: 55
}
```

## 2. `while` Loop

The `while` loop is used when you want to repeat a block of code an unknown number of times, but you have a condition that determines when to stop.

### Syntax:
```javascript
while (condition) {
    // code block to be executed
}
```

### When to Use:
- When you don't know exactly how many iterations you need, but you have a condition to check.
- Example: Looping until a variable is greater than 5.

### Examples:

1. **Basic `while` loop from 1 to 5:**
```javascript
let count = 1;
while (count <= 5) {
    console.log(count);  // Output: 1 2 3 4 5
    count++;
}
```

2. **Sum of numbers 1 to 10:**
```javascript
let total = 0;
let i = 1;
while (i <= 10) {
    total += i;  // Adds numbers 1 to 10
    i++;
}
console.log(total);  // Output: 55
```

3. **Countdown from 10 to 1:**
```javascript
let number = 10;
while (number > 0) {
    console.log(number);  // Output: 10 9 8 7 6 5 4 3 2 1
    number--;
}
```

4. **Product of numbers 1 to 5:**
```javascript
let result = 1;
let i = 1;
while (i <= 5) {
    result *= i;  // Multiplies 1*2*3*4*5
    i++;
}
console.log(result);  // Output: 120
```

5. **Sum of even numbers from 2 to 20:**
```javascript
let total = 0;
let i = 2;
while (i <= 20) {
    total += i;  // Adds even numbers from 2 to 20
    i += 2;
}
console.log(total);  // Output: 110
}
```

## 3. `do...while` Loop

The `do...while` loop is similar to the `while` loop, but it guarantees that the block of code will run at least once before checking the condition.

### Syntax:
```javascript
do {
    // code block to be executed
} while (condition);
```

### When to Use:
- When you want the loop to execute at least once, regardless of the condition.
- Example: Asking a user for a correct input until it's valid.

### Examples:

1. **Basic `do...while` loop from 1 to 5:**
```javascript
let count = 1;
do {
    console.log(count);  // Output: 1 2 3 4 5
    count++;
} while (count <= 5);
```

2. **Sum of numbers 1 to 10:**
```javascript
let sum = 0;
let i = 1;
do {
    sum += i;  // Adds numbers 1 to 10
    i++;
} while (i <= 10);
console.log(sum);  // Output: 55
```

3. **Countdown from 10 to 1:**
```javascript
let number = 10;
do {
    console.log(number);  // Output: 10 9 8 7 6 5 4 3 2 1
    number--;
} while (number > 0);
```

4. **Sum of squares of numbers 1 to 5:**
```javascript
let total = 0;
let i = 1;
do {
    total += i * i;  // Adds the square of each number
    i++;
} while (i <= 5);
console.log(total);  // Output: 55
```

5. **Product of numbers 1 to 5:**
```javascript
let result = 1;
let i = 1;
do {
    result *= i;  // Multiplies 1*2*3*4*5
    i++;
} while (i <= 5);
console.log(result);  // Output: 120
```

## 4. `switch` Statement

A `switch` statement is used when you need to execute one out of multiple possible code blocks, depending on the value of an expression.

### Syntax:
```javascript
switch (expression) {
    case value1:
        // code block
        break;
    case value2:
        // code block
        break;
    default:
        // default code block if no match
}
```

### When to Use:
- When you have multiple conditions and want to simplify if-else chains.
- Example: Checking different days of the week.

### Examples:

1. **Checking the day of the week:**
```javascript
let day = 3;
switch (day) {
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    case 3:
        console.log("Wednesday");  // Output: Wednesday
        break;
    default:
        console.log("Invalid day");
}
```

2. **Checking a number:**
```javascript
let number = 2;
switch (number) {
    case 1:
        console.log("One");
        break;
    case 2:
        console.log("Two");  // Output: Two
        break;
    case 3:
        console.log("Three");
        break;
    default:
        console.log("Not a valid number");
}
```

3. **Checking a color:**
```javascript
let color = "red";
switch (color) {
    case "red":
        console.log("The color is red");  // Output: The color is red
        break;
    case "blue":
        console.log("The color is blue");
        break;
    default:
        console.log("Unknown color");
}
```

4. **Grade based on score:**
```javascript
let score = 85;
switch (true) {
    case (score >= 90):
        console.log("Grade A");
        break;
    case (score >= 80):
        console.log("Grade B");  // Output: Grade B
        break;
    case (score >= 70):
        console.log("Grade C");
        break;
    default:
        console.log("Fail");
}
```

5. **Checking fruit:**
```javascript
let fruit = "apple";
switch (fruit) {
    case "banana":
        console.log("It's a banana");
        break;
    case "apple":
        console.log("It's an apple");  // Output: It's an apple
        break;
    default:
        console.log("Unknown fruit");
}
```
```

