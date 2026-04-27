1. Line 12 prints ```3``` to the console, which is the number of elements in the array passed into ```discountPrices```. The for loop iterates once for each element in the array, and ```i``` equals the length of the array after the for loop terminates.
2. Line 13 prints ```150``` to the console. This is the discounted price of the third item in the array. After the for loop termaintes, the variable ```discountedPrice``` is still holding this value.
3. Line 14 prints ```150``` to the console. This is the value stored in ```finalPrice``` after the for loop terminates.
4. The call to ```discountPrices``` returns an array with the values ```[50, 100, 150]```. This is the result of applying the 0.5 discount value to the argument array with values ```[100, 200, 300]```.
5. Line 12 causes an error, since ```i``` is now a block-scoped variable that only exists in the for loop, and is not in the scope of this line.
6. Line 13 also causes an error, since ```discountedPrice``` is now a block-scoped variable that only exists in the for loop, and is not in the scope of this line.
7. Line 14 prints ```150``` to the console. Changing ```finalPrice``` to a block-scoped variable didn't cause any errors because it's in the same block and has the same scope as line 14.
8. This code returns the same array from question #4, with values ```[50, 100, 150]```. Since the code is relatively simple, changing the variables from function to block scope didn't have any effects on the execution of the program.
9. Same as in question #5, line 11 causes an error, since ```i``` is now a block-scoped variable that only exists in the for loop, and is not in the scope of this line.
10. Line 12 prints ```3``` to the console. This is the length of the array ```prices```, which was found on line 4.
11. This code returns the same array from question #4, with values ```[50, 100, 150]```. Making ```discounted``` a constant still lets us add elements with ```push```, so this code runs with no errors.
12. - A) ```student.name```
	- B) ```student["Grad Year"]```
	- C) ```student.Greeting()```
	- D) ```student["Favorite Teacher"].name```
	- E) ```student.courseLoad[0]```
13. - A) ```32```. When using ```+``` to add a string and an int, Javascript converts the int to a string and concatenates them.
	- B) ```1```. For other arithmetic operations between strings and ints, Javascript converts the string into an int and performs the arithmetic.
	- C) ```3```. The null value in Javascript is "falsy" and converts to the integer value 0.
	- D) ```3null```. The null value in Javascript converts to the string value "null".
	- E) ```4```. The ```true``` keyword in Javascript is truthy and converts to the integer 1.
	- F) ```0```. The ```false``` keyword in Javascript is falsy and converts to the integer 0. This is added with null, another 0.
	- G) ```3undefined```. Javascript creates a string "undefined" when you try to convert an undefined value to a string.
	- H) ```NaN```. This is "not a number", since the undefined value in Javascript doesn't have any numerical represnetation.
14. - A) ```true```. Javascript converts the string ``` `2` ``` into an integer, which is greater than 1.
	- B) ```false```. Since both arguments are strings, Javascript does string-to-string comparison, which is based on alphabetical order.
	- C) ```true```. When comparing values with different types, Javascript converts the values to numbers. This makes the string ``` `2` ``` convert into the integer 2.
	- D) ```false```. When *strictly*  comparing values with different types, Javascript doesn't do any type conversion, and sees that ``` `2` ``` the string and ```2``` the number are different objects.
	- E) ```false```. Javascript converts ```true``` here into the number 1, which does not equal 2.
	- F) ```true```. ```Boolean(2)``` returns the boolean value ```true```, since 2 is nonzero.
15. The == operator implicity converts arguments with different types into numbers, then compares the numbers. The === operator returns ```false``` immediately if the arguments are different types, and only compares the arguments if they have the same type.
16. See ```part2-question16.js```
17. The function ```modifyArray``` runs the function provided by ```callback``` on the values 1, 2, and 3, and stores the return values of ```callback``` on each of those values inside of ```newArr```. In this case, the callback function returns the value multiplied by 2, so ```newArr``` contains the values 2, 4, and 6.
18. See ```part2-question18.js```
19. ```1``` <br> ```4``` <br> ```3``` <br> ```2```