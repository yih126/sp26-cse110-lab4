## 1. What will happen at line 12 and why?

**3**

The variable `i` is declared using `var`, which has function scope. Even though `i` is declared inside the `for` loop, it is still accessible outside the loop. After the loop finishes, `i` becomes 3 (the length of the array), so line 12 prints 3.

## 2. What will happen at line 13 and why?

**150**

The variable `discountedPrice` is declared using `var`, which has function scope. Even though it is declared inside the loop, it is still accessible outside the loop. After the loop finishes, `discountedPrice` holds the last computed value (for 300), which is 150, so line 13 prints 150.

## 3. What will happen at line 14 and why?

**150**

The variable `finalPrice` is declared using `var`, which has function scope. It is updated during each iteration of the loop, and after the loop finishes, it holds the last computed value (150), so line 14 prints 150.

## 4. What will this function return?

**[50, 100, 150]**

The function loops through the `prices` array and applies the discount to each value. Each discounted value is rounded to two decimal places and pushed into the `discounted` array. Finally, the function returns this array.

## 5. What will happen at line 12 and why?

**ReferenceError (i is not defined)**

The variable `i` is declared using `let`, which has block scope. It only exists inside the `for` loop, so it is not accessible outside the loop. Therefore, line 12 causes a ReferenceError.

## 6. What will happen at line 13 and why?

**ReferenceError (discountedPrice is not defined)**

The variable `discountedPrice` is declared using `let`, which has block scope. It only exists inside the `for` loop, so it is not accessible outside the loop. Therefore, line 13 causes a ReferenceError.

## 7. What will happen at line 14 and why?

**150**

The variable `finalPrice` is declared with `let` at the function level, not inside the `for` loop. Because line 14 is still inside the same function, it can access `finalPrice`. After the loop finishes, `finalPrice` holds the last calculated value, which is 150.

## 8. What will this function return?

**[50, 100, 150]**

The function loops through the `prices` array, applies the discount to each value, rounds it, and stores it in the `discounted` array. Since `finalPrice` is declared outside the loop (but inside the function), it can be updated and used correctly. The function returns the array of discounted prices.

## 9. What will happen at line 11 and why?

**ReferenceError (i is not defined)**

The variable `i` is declared using `let`, which has block scope. It only exists inside the `for` loop, so it is not accessible outside the loop. Therefore, line 11 causes a ReferenceError.

## 10. What will happen at line 12 and why?

**3**

The variable `length` is declared using `const` at the function scope. Since it is not inside the loop, it is accessible at line 12. The value of `length` is 3 (the length of the array), so line 12 prints 3.

## 11. What will this function return?

**[50, 100, 150]**

The function loops through the `prices` array and applies the discount to each value. Each discounted value is added to the `discounted` array. Since all variables are used within their correct scope, the function runs without errors and returns the array of discounted prices.

## 12.

A. student.name

B. student['Grad Year']

C. student.greeting()

D. student['Favorite Teacher'].name

E. student.courseLoad[0]

## 13. Arithmetic

A. '3' + 2  
**'32'**  
String concatenation: number is converted to string.

B. '3' - 2  
**1**  
Subtraction forces numeric conversion.

C. 3 + null  
**3**  
null converts to 0.

D. '3' + null  
**'3null'**  
String concatenation.

E. true + 3  
**4**  
true converts to 1.

F. false + null  
**0**  
false → 0, null → 0.

G. '3' + undefined  
**'3undefined'**  
String concatenation.

H. '3' - undefined  
**NaN**  
undefined cannot convert to number.


## 14. Comparison

A. '2' > 1  
**true**  
String converts to number (2 > 1).

B. '2' < '12'  
**false**  
String comparison.

C. 2 == '2'  
**true**  
Loose equality converts types.

D. 2 === '2'  
**false**  
Strict equality checks type and value.

E. true == 2  
**false**  
true → 1, 1 ≠ 2.

F. true === Boolean(2)  
**true**  
Boolean(2) → true, same type and value.


## 15. Difference between == and ===

`==` compares values after type conversion (loose equality).  
`===` compares both value and type without conversion (strict equality).

## 17. The result is [2, 4, 6].

The function iterates through each element in the array and applies the callback function doSomething, which multiplies each number by 2. The results are stored in a new array and returned.

## 19.
1  
4  
3  
2  

The synchronous code runs first (1 and 4). Then the setTimeout with 0ms executes (3), followed by the setTimeout with 1000ms (2).