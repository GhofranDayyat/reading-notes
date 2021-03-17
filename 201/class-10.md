# CH10 : Errors Handling and Debugging

 **THE STACK**
 the java script interpreter processes one line of code at a time. when a statement needs data from another function ,its stacks the new function on top of the current task

* **Debugging** :Debugging is the process of finding errors. It involves a process of deduction
* To find the error in your code  you must understand execution contexts (which have two stages) and stacks, you are more likely to 
* You can try to find the exact error by The console it's helps narrow down the area in which the
error is located.
* JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.
* If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.

## Execution contexts
1. GLOBAL CONTEXT: Code that is in the script, but not in a function. There is only one global context in any page.
2. FUNCTION CONTEXT: Code that is being run within a function. Each function has its own function context.
3. EVAL CONTEXT: Text is executed like code in an internal function called eval().(NOT SHOWN)

## Error Objects:
1. Error
2. SyntaxError
3. ReferenceError
4. TypeError
5. RangeError
6. URIError
7. EvalError 
8. name 
9. message
10. fileNumber
11. lineNumber

## Error Types

* Syntax Error: Incorrect syntax 
* Reference Error: variable doesn't exist 
* URI Error: Incorrect use of URI function 
* Eval Error: Incorrect use of eval() function 
* Type Error: value is unexpected data type 
* Range Error: number outside of range 
* Error: genaric error object 
* NaN: not a number
