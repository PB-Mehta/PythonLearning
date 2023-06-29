1. What are the two values of the Boolean data type? How do you write them? 
_ANS._ boolean data types returns true or false for example
for example type(False) type(True)


2. What are the three different types of Boolean operators?
_ANS._ AND (botn true)
       OR  (any one true)
       NOT (negation)


3. Make a list of each Boolean operator's truth tables (i.e. every possible combination of Boolean values for the operator and what it evaluate ).
_ANS._ AND TRUTH TABLE
x	    and	y	    Returns
True	and	True	True
True	and	False	False
False	and	True	False
False	and	False	False
OR TRUTH TABLE
x	    or	y	    Returns
True	or	True	True
True	or	False	True
False	or	True	True
False	or	False	False
NOT TRUTH TABLE 
not	x	    Returns
not	True	False
not	False	True

4. What are the values of the following expressions?
(5 > 4) and (3 == 5)                   ans. false
not (5 > 4)                            ans. true
(5 > 4) or (3 == 5)                    ans. true
not ((5 > 4) or (3 == 5))              ans. false
(True and True) and (True == False)    ans. false
(not False) or (not True)              ans. true


5. What are the six comparison operators?
==  Equal to
!=	Not equal to
<	Less than
>	Greater than
<=	Less than or equal to
>=	Greater than or equal to


6. How do you tell the difference between the equal to and assignment operators?Describe a
condition and when you would use one.
_ANS._ equal is used to assign the value where as == is used to compare the right operand to its left operand when needed to check the vales or compare the == should be used else for assignment use =

7. Identify the three blocks in this code:
spam = 0
if spam == 10:
print('eggs')
if spam > 5:
print('bacon')
else:
print('ham')
print('spam')
print('spam')
_ANS._if block then print('spam') and print('spam')
8. Write code that prints Hello if 1 is stored in spam, prints Howdy if 2 is stored in spam, and prints
Greetings! if anything else is stored in spam.
_ANS._ 
spam = 0
if spam == 1:
    print('Hello')
    if spam == 5:
        print('howdy')
    else:
        print('Greetings!')


9. If your programme is stuck in an endless loop, what keys you’ll press?
_ANS._ ctrl+c


10. How can you tell the difference between break and continue?
_Ans._ break statement is used to terminate the loop when condition returns true 
while continue statement skips the code for that current iteration 



11. In a for loop, what is the difference between range(10), range(0, 10), and range(0, 10, 1)?
_Ans._ 
all the output will be same 
range(10) 0 to 10
range(0,10) start from zero end to 10 numbers
range (0,10,1) start from zero to 10 numbers with each step at 1


12. Write a short program that prints the numbers 1 to 10 using a for loop. Then write an equivalent program that prints the numbers 1 to 10 using a while loop.
_Ans._ 
for i in range(1,10):
    print(i)

i = 1
while(i<=10):
    print(i)
    i += 1    


13. If you had a function named bacon() inside a module named spam, how would you call it after importing spam?
_ANS._ spam.bacon()