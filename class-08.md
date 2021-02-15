# CH5 Layout
## Key Concepts in Positioning Elements
* CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box
- Block-level boxes start on a new line and act as the main building blocks of any layout
- inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes , To separate boxes, you can use borders, margins, padding, and background colors.

* **Containing Elements**: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

## Controll ing the Position of El ements

CSS has the following positioning schemes that allow you to control the layout of a page: 
1. normal flow
2. relative positioning
3. absolute positioning. 
* You can also float elements using the float property.

## box offset
* To indicate where a box should be positioned,properties to tell the browser how far from the top or bottom
and left or right it should be placed.
* When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top,There are two types:

1. Fixed Positioning
2. Floating Elements

## Screen Sizes
Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

## Screen Resolution
Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens
## Page Sizes
Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).

## Fixed Width Layouts
Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.

## Liquid Layouts
Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.
## Summary
* ```<div>``` elements are often used as containing elements to group together sections of a page.
* Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.
* The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)
* Pages can be fixed width or liquid (stretchy) layouts
* Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).
* Grids help create professional and flexible designs
* CSS Frameworks provide rules for common tasks.
* You can include multiple CSS files in one page. 