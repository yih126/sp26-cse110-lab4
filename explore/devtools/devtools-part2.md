# DevToolsDevTools - Debugging
1. The bug was that num1 and num2 are strings, so the "+" operator performs string concatenation instead of numeric addition.1. 
2. To fix it, convert the inputs to numbers using Number() before adding them.