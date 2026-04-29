# Debugging Process (Expand Section)

In this part, I used Chrome DevTools to debug the JavaScript code.

First, I opened the Sources tab and set a breakpoint at the line where the variable `result` is initialized inside the `calculateSum()` function.

Then, I clicked the "Calculate Sum" button on the webpage, which triggered the debugger and paused execution at the breakpoint.

Next, I added watch expressions to observe the values of `num1`, `num2`, and the data type of `result`.

I noticed that both `num1` and `num2` were strings (for example, "2" and "3"), which caused the `+` operator to perform string concatenation instead of numeric addition. This resulted in "23" instead of 5.

To fix this issue, I converted the inputs to numbers using `Number(num1)` and `Number(num2)` before adding them.

After applying the fix, the program correctly calculated the sum.