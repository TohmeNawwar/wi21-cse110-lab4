1. Since var has no block scoepe, line 11 will print the value of i to console
2. Since var has no block scope, the variable persists after the for loop and the value of discountedPrice will be printed to console.
3. Since var has no block scope, line 13 will print the value of finalPrice to console.
4. If we call discountPrices([100, 200, 300]), .5), the function will return [50, 100, 150], because it will loop through the for loop, and update discounted with each halved price, since the discount is .5
5. Here, line 11 would return an error, as variable i is defined with let in the for loop, and so will only have block scope and will not be visible outside of the for loop.
6. Line 12 would also return an error for the same reason as line 11, as discountedPrice is defined in the for loop with let and so will not be visible to log in line 12 outside of the loop.
7. Line 13 would print the value of finalPrice to console, as finalPrice is declared at the beginning of the function in which it is printed, rather than within a different block, and so is visible to be printed in line 13.
8. The function will return not return anything for discountPrices([100, 200, 300], .5), as it will have an error at lines 11 or 12 stopping it from running. However, assuming these worked, it would return [50, 100, 150].
9. At line 11, an error would be returned, as variable i is defined with let in the for loop and so will have a block scope limited within the for loop and not be visible outside of it.
10. Line 12 would print the first value of discountedPrice, as it is a const variable which cannot be updated after the first value it is assugned
11. Line 13 would return an error, as discountedPrice is declared in the foor loop as a const and so is outside of the scope of line 12, and is not visible here.
12. The function would return nothing for discountPrices([100, 200, 300], .5), as there would be errors trying to update the const variables. However, if the code were to run past these errors, the function would return [], as discounted cannot be updated after its declaration since it is a const variable.
13.
    1. student.name
    2. student['Grad Year']
    3. student.greeting()
    4. student['Favorite Teacher'].name
    5. student.courseLoad[0]
14.
    1. '3' + 2 outputs '32', + operator converts both operands to a string if one is a string.
    2. '3' - 2 outputs 1, - operator converts both operands to numbers
    3. 3 + null = 3, null gets converted to 0
    4. '3' + null = '3null', null gets converted to string before addition
    5. true + 3 = 4, true gets converted into 1 when converted to a number
    6. false + null = 0, false and null both get converted to 0
    7. "3" + undefined = '3undefined', since '3' is a string, + converts undefined to be a string and concatenates.
    8. "3" - undefined = NaN, since undefined gets converted to NaN when converted to a number
15.
    1. '2' > 1 returns true, as the 2 gets converted to a number which is less that 2, so returns true
    2. '2' < '12' returns false, since both are strings the first char in 2 gets compared to the first char in 12, and since 2 is not less than 1, returns false
    3. 2 == '2' returns true, since the string '2' gets converted to the number 2 and 2 == 2 is true
    4. 2 === '2' returns false, since === does not convert the types and since 2 and '2' are different types 2 === '2' returns false
    5. true == 2 returns false, since true gets converted to the number 1 and 1 does not equal 2
    6. true === Boolean(2) returns true, since 2 is not an empty value, Boolean(2) converts 2 to true and true === true.
16. == will convert different types to numbers, while === is strict equality which will check equality without type conversion, and so will be false if comparing two different types.
17. 'How are you?' gets printed, since 2 == true is false, as true gets converted to 1 and 2 does not equal 1, and so 'Hello!' is not printed. Instead, in the else if statement, the 2 gets converted to a boolean, and since it 2 is a non empty value, it gets converted to true, so the code in the else if gets executed.
18. See part1-question18.js
19. The result will be [6, 8, 10], because modifyArray will call doSomething with parameters num and a function which doubles input for each num in the input array [1, 2, 3] Do something then adds 2 to the number input and returns it run through the input callback function, which doubles the input. So 2*(1 + 2) = 6, 2*(2 + 2) = 8, 2*(3 + 2) = 10.
20. See part1-question20.js
21. This code will output 1 4 3 2, because it will first run 1, then put a timer to print 2 which takes 1 second, then a timer to print 3 which takes 0 seconds, then print 4 to console. In this time, it prints 4 before executing either and 3 before printing 2.
