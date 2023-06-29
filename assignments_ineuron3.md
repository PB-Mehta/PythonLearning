1. Why are functions advantageous to have in your programs?
_ANS._ functions can be used multiple times without writing its whole code multiple times for same logic or return value


2. When does the code in a function run: when it's specified or when it's called?
_ANS._ when its called

3. What statement creates a function?
_ANS._ First we need to declare the function just as we do with variable followed by defining it syntax-
def name():
    task

4. What is the difference between a function and a function call?
_ANS._function is only written once while a funtion call may be invoked multiple times in the same code 


5. How many global scopes are there in a Python program? How many local scopes?
_ANS._ there is only one global scope in python 


6. What happens to variables in a local scope when the function call returns?
_ANS._ every time function is called new local variable is formed and returns to that caller 


7. What is the concept of a return value? Is it possible to have a return value in an expression?
_ANS._ values passed by a function call are recieved to the funtion code where operations are done and at the end the final value is returned to the funtion where it is called moreover type conversion may be needed as passed and returned must be compatible


8. If a function does not have a return statement, what is the return value of a call to that function?
_ANS._ last statement of he called funtion is executed and the return is undefined 


9. How do you make a function variable refer to the global variable?
_ANS._ by using global keyword in front of variable name 


10. What is the data type of None?
_ANS._ none type


11. What does the sentence import areallyourpetsnamederic do?
_ANS._ import keyword id used to import a module or library if  areallyourpetsnamederic exists then it will do import


12. If you had a bacon() feature in a spam module, what would you call it after importing spam?
_ANS._ spam.bacon() 
13. What can you do to save a programme from crashing if it encounters an error?
_ANS._ different error handling techniques can be used such as break  statements , try except finnaly blocks , continue etc.


14. What is the purpose of the try clause? What is the purpose of the except clause?
_ANS._ try clause tests the block of code for errors while except lets us handle the error 