```markdown
# 2-Day Quiz Project by Assey

This project consists of three different coding challenges. Each challenge is designed to test your understanding of JavaScript and basic programming concepts.

---
```

## Question 1: **Print " I Love JS" Using Asterisks**

### **Objective:**
Create a program that prints the phrase **"I Love JS"** using `console.log()` and asterisks (`*`) in such a way that each letter of the phrase forms a recognizable shape. Use functions for each letter.

### **Requirements:**
- Write a function to print each letter of **"I Love JS"** (i.e., "I", "L", "O", "V", "E", "J", "S").
- Use `console.log()` to print each line of the pattern.
- Each letter should be represented using asterisks (`*`).
- The output should visually look like the word **"I Love JS"**.

### **Hint:**
Begin with simple patterns for each letter, then combine them to form the full phrase.

  ---
```
---
```
### Question 2: **RAM Diagram and Variable Scope**

### **Objective:**
Draw a RAM diagram to visualize the variable declaration and scope in the following code. Also, explain the scope of each variable.

### **Code:**```


   ```javascript
let a = 5;
function checkNumber() {
    let b = 10;
    if (a < b) {
        let c = 15;
        console.log(a, b, c);
    }
    console.log(a, b);
}
checkNumber();
console.log(a);
```

### **Requirements:**
1. Draw the RAM diagram showing how variables `a`, `b`, and `c` are stored in memory.
2. Identify the scope of each variable and explain where each variable is accessible in the code.
3. After running the function `checkNumber()`, determine which variables will be accessible outside the function.

### **Hint:**
Pay attention to the function scope and block scope for variables `b` and `c`.

---

## Question 3: **Food Menu Checker App**

### **Objective:**
Create a program that checks what food should be eaten based on the day of the week. The program should use a function to determine the food based on the current day.

### **Requirements:**
1. Write a main function that takes the current day (e.g., "Monday", "Tuesday") and checks what food is associated with it.
2. Use `if/else` or `nested if` statements to return a food item for each day.
3. The days of the week should have a unique food item associated with them. For example, Monday could be "Pizza", Tuesday could be "Burger", and so on.
4. If an invalid day is entered, return an error message.

### **Hint:**
The program should simulate the current day (for example, you can hardcode the day as `"Monday"` to test).

---

Good luck with your quiz!
```

