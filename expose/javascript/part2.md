1. Line 12 prints `3` because `i` was declared with `var`, meaning it is still accessible outside the `for loop`. After the loop finishes, `i` equals `3` since it has incremented past the last index (2). 
2. Line 13 prints `150` because `discountedPrice` was declared with `var`, meaning it is still accessible outside the `for loop`. Its final value comes from the last iteration, where `300 * 0.5 = 150`.
3. Line 14 prints `150` because `finalPrice` was declared with `var`, meaning it is still accessible outside the `for loop`. Its final value is from the last iteration after rounding the discounted price of `300` by 50%, `150`.
4. This function returns `[50, 100, 150]` because each price in the array is reduced by the 50% discount, rounded, and pushed into the `discounted` array during each loop iteration. After the loop finishes, the array of discounted prices is returned.
5. Line 12 throws a **ReferenceError: i is not defined** error because `i` was declared with `let`, which is block-scoped to the `for` loop. Once the loop ends, `i` no longer exists outside that block and `console.log(i);` is called after the loop ends.
6. Line 13 throws a **ReferenceError: discountedPrice is not defined** because `discountedPrice` is declared with `let` inside the `for` loop, making it block-scoped and inaccessible outside the loop.
7. Line 14 prints `150` because `finalPrice` is updated on each loop iteration and ends with the last computed value (from `300 * 0.5`). Since `finalPrice` is declared with `let` in the function scope, it is accessible and retains its final updated value.
8. This function returns `[50, 100, 150] `because each price is discounted, rounded, and pushed into the `discounted` array during the loop. Since `discounted` is declared with `let` in the function scope, it is accessible and retains its final updated value.
9. Line 11 throws a **ReferenceError: i is not defined** because `i` is declared with `let` inside the `for` loop, making it block-scoped and only accessible within that loop. Once the loop ends, `i` no longer exists outside the block.
10. Line 12 prints `3` because `length` is a constant storing `prices.length`, which is 3 for the given input array. Since `const length` is declared in the function scope, it is accessible throughout the function and retains its value.
11. This function returns `[50, 100, 150]` because it loops through each price, applies the discount, and stores each result in the `discounted` array. Although `discounted` is declared with `const`, meaning it cannot be reassigned, it's contents (pushing into the array) can still be updated. After all iterations, the completed array is returned.
12. 
    A. student.name 
    B. student["Grad Year"]
    C. student.greeting()
    D. student["Favorite Teacher"].name
    E. student.courseLoad[0]

13. 
    A. '32' Because + with a string triggers concatenations, so 2 is converted to a string since integers map to their exact string representaiton. 
    B. 1 Because - forces numeric conversion, so "3" becomes 3.
    C. 3 Because null is treated as 0 in numeric operations 
    D. '3null' Because strong concatenation occurs, so null becomes "null"
    E. 4 Because true maps to 1
    F. 0 Because both false and null map to 0.
    G. "3undefined" string concacatenation occurs, sno undefined becomes "undefined"
    H. NaN undefined becomes NaN, and any math with NaN stays NaN.

14. 
    A. true because '2' is converted to number 2
    B. false because string comparison is lexicongraphic, so "2" is greater than "1"
    C. true because == allows type coercion, so both become 2
    D. false becuase === checks value and type, so number != string 
    E. false because true maps to 1, so 1 == 2 is false
    F. true because Boolean(2) is true, and both are the same type and value

15. == compares values after converting types (loose equality), while === compares both value and type without conversion (strict equality).

16. see part2-question16.js

17. `modifyArray` loops through each element of `[1, 2, 3]` and applies the callback function `doSomething` to each value. `doSomething(num)` returns `num * 2`, so each number is doubled: 1 --> 2, 2 --> 4, 3 --> 6. These results are pushed into `newArr`, which is then returned.

18. see part2-question18.js

19. 
1
4
3
2