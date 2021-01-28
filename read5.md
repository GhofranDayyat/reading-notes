# Comparison Operators Evaluating Condition

## You can evaluate a situation by comparing one value in the script to what you expect it might be. The result will be a Boolean: true or false.

* Programmers refer to the testing or checking of a condition as evaluating the condition. Conditions can be much more complex than those shown here, but they usually result in a value of true or false.

**==** _ IS EQUAL TO _
 This operator compares two values (numbers, strings, or Booleans) to see if they are the same.. "Hello' == 'Goodbye' returns false because they are not the same string. "Hello == Hello' returns true because they are the same string. It is usually preferable to use the strict method
 
 **!=** _ IS NOT EQUAL TO _
  This operator compares two values (numbers, strings, or Booleans) to see if they are not the same. 'Hello = 'Goodbye' returns true because they are not the same string. "Hello 'Hello' returns false because they are the same string. It is usually preferable to use the strict method 
  
  **===** _ STRICT EQUAL TO _
  This operator compares two values to check that both the data type and value are the same. 3 3returns false because they are not the same data type or value. 3' '3' returns true because they are the same data type and value.

**==!** _ STRICT NOT EQUAL TO _
 This operator compares two values to check that both the data type and value are not the same. '3' == 3 returns true because they are not the same data type or value. '3 1= '3 returns false because they are the same data type and value.

 **>** _ GREATER THAN _
 This operator checks if the number on the left is greater than the number on the right. 4>3 returns true 3> 4 returns false

 **<** _LESS THAN OR EQUAL TO _
  This operator checks if the numberon the left is less than or equal to the number on the right.
**>=** _ GREATER THAN OR EQUAL TO _ 
This operator checks if the number on the left is greater than or equal to the number on the right.
**<=** _ LESS THAN OR EQUAL TO _
 This operator checks if the numberon the left is less than or equal to the number on the right.


## LOGICAL OPERATORS 
Comparison operators usually return single values of true or false. Logical operators allow you to compare the results of more than one comparison operator.
* LOGICAL **AND** _ && _ This operator tests more than one condition
* LOGICAL **OR** _||_ This operator tests at least one condition
* LOGICAL **NOT** _!_  This operator takes a single Boolean value and inverts it.


|A | B| &&   |  || |                                                                      
|--|--|------|-----|
|T |T |  T   |  T  |             
|T |F |  F   |  T  |                        
|F |T |  F   |  T  |                 
|F |F |  F   |  F  |

## Short_Circuit Evaluation
* F && anything it get false
* T || anything it get true


# LOOPS 
Loops check a condition. If it returns true, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. It repeats until the condition returns false. There are three common types of loops:

1. **FOR** 
If you need to run code a specific number of times, use a for lop. (It is the most common loop.) In a for loop, the condition is usually a counter which is used to tell how many times the loop should run.

```
for (var i = 0 < 10 ; i++ ){
  document.write(i);
}
```
 _Result_ :1 2 3 4 5 6 7 8 9 10\
 * the loop comsisting of:
 - Initalization : var i = 0;
 - Condition: i < 10;
 - Update :i++



 
2. **WHILE If**
you do not know how many times the code should run, you can use a while loop. Here the condition can be something other than a counter, and the code will continue to loop for as long as the condition is true. 

```
var i = l ;
var msg = ' ' ;
while (i < 10) {
msg += i + ' x 5 = ' + (i * 5) + '<br I>';
i++;
document .getEl ementByid( ' answer') . innerHTML = msg;
```
* Result: lxS=S
2 x s = 10
3 x 5 = 15 .
4 x 5 = 20
s x s = 25
6 x s = 30
7 x 5 = 35
8 x s = 40
9 x 5 = 45 
* Inside the code block there are
two statements: 
- The first statement uses the+=
operator
- The second statement
increments the counter variable
by one
3. **DO.. WHILE**
 The do...while loop is very similar to the wh1le loop, but has one key difference: it will always run the statements Inside the curly braces at least once, even if the condition evaluates to false.


 