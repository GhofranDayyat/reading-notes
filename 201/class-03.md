# CH3 Links to an external site
## types of lists in html
1.	ordered list (ol)
2.	unordered list (ul)
3.	defintion list (dl)

**unorder List**
created with the element 
```< ul > < li > < /li> < /ul >```result will apper with dot
**definition List**
 created with the element and usually consists of a series of terms and their definitions. ```< dl > < dt > < dd > < /dd> < /dt> < /dl >```

**The ordered list**
  created with the element ```< ol > < li > < /li> < /ol >```result well apper ordered 1- 2- 3-

  ## Summary
* here are three types of HTML lists: ordered, unordered, and definition.
* Ordered lists use numbers.
* Unordered lists use bullets.
* Definition lists are used to define terminology.
* Lists can be nested inside one another.
# CH13: “Boxes”
## properties OF Boxes
1. *Border* Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another
2. *MarginMargins* sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
3. *Padding* : is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.

## over flowing content The overflow property tells the browser what to do if the content contained within a box is larger than the box itself
* hidden
* scroll
## Box dimensions 
The most popular ways to specify the size of a box are to use pixels, percentages, or ems
## limitng width
1. min-width :the smallest size a box can be displayed at when the browser window is narrow
2. max-width :the maximum width a box can stretch to when the browser window is wide
## limiting hight 
1. mini height
2. max height

## Summary
* CSS treats each HTML element as if it has its own box.
* You can use CSS to control the dimensions of a box.
* You can also control the borders, margin and padding for each box with CSS.
* It is possible to hide elements using the display and visibility properties.
* Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
* Legibility can be improved by controlling the width of boxes containing text and the leading.
* CSS3 has introduced the ability to create image borders and rounded borders.


# CH2 Basic JavaScript Instructions
## ARRAYSAn 
**array is a special type of variable. It doesn’t just store one value; it stores a list of values**

## VALUES IN ARRAYS
1. NUMBERING ITEMS IN AN ARRAY Each item in an array is automatically given a number called an index
2. ACCESSING ITEMS IN AN ARRAY To retrieve the third item on the list, the array name is specified along with the index number in square brackets
3. NUMBER OF ITEMS IN AN ARRAY Each array has a property called length, which holds the number of items in the array

**ACCESSING & CHANGING VALUES IN AN ARRAY** The first lines of code on the leftcreate an array containing a list of three colors. (The values can be added on the same line or on separate lines as shown here.Having created the array, the third item on the list changed from 'custom' to 'beige'

# CH4 Decisions and Loops
**Loops** Loops check condition and if it true a code will run until it false we have more than one type of loop:
1. for loop (for loop is often used to loop through the items in an array. )
2. while loop
3. do while loop (The key difference between a whi 1 e loop and a do whi 1 e loop is that the statements in the code block come before the condition. This means that those statements are run once whether or not the condition is met. 
## Summary
* Conditional statements allow your code to make decisions about what to do next.
* Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>) are used to compare two operands.
* Logical operators allow you to combine more than one set of comparison operators.
* if ... else statements allow you to run one set of code if a condition is true, and another if it is false.
* switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match).
* Data types can be coerced from one type to another.
* All values evaluate to either truthy or falsy.
* There are three types of loop: for, while, and do ... while. Each repeats a set of statements.


