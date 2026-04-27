1. ```values added:	20```
2. ```final result: 20```
3. Variables declared with ```var``` have "function scope", meaning that they are defined everywhere inside their function. This is different from ```let```, which gives variables "block scope". A variable with block scope only exists inside of its block, such as an ```if``` expression. Block scope is much more popular and well-understood than function scope in modern programming languages, so we should try to use ```let``` instead of ```var```.
4. ```values added:	20```
5. This throws an error, since ```result``` has block scope and is not in the scope of this line.
6. This line isn't reached, because the code returns an error in a previous line. This is because we re-assign the value of ```result```, even though it's a constant.
7. This line also isn't reached, because the code returns an error in a previous line. This is because we re-assign the value of ```result```, even though it's a constant.