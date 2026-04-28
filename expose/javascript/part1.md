## 1. What is printed by line 9?

**values added: 20**

Since `add` is true, the `if` block runs and `result` is set to `num1 + num2 = 20`, so line 9 prints this value.


## 2. What is printed by line 13?

**final result: 20**

The variable `result` is declared using `var`, which has function scope, so it is accessible outside the `if` block. Therefore, line 13 can print it.


## 3. Why should you not use var?

`var` should be avoided because it has function scope instead of block scope, which can lead to unexpected behavior and bugs.


## 4. What is printed by line 9?

**values added: 20**

Since `add` is true, the `if` block runs and `result` is calculated as 10 + 10 = 20. Line 9 is inside the block, so it can access `result`.


## 5. What is printed by line 13?

**ReferenceError**

`result` is declared with `let`, which has block scope. It only exists inside the `if` block, so line 13 cannot access it.

## 6. What is printed by line 9?

**Error**

`result` is declared with `const`, so it cannot be reassigned. The line `result = num1 + num2;` causes an error before line 9 executes, so nothing is printed.


## 7. What is printed by line 13?

**Nothing**

Since the error occurs before line 9, the function stops executing, so line 13 is never reached.