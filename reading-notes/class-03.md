# List in HTML
There are lots of methods to make a list.
HTML provides 3 types of list :
* Ordered list
* Unordered list
* Definition list 

**Ordered list**

List where each item in the list is numbered.

It is created with <*ol>* element.

Each item in the list is placed by using <*li>* element.


**Unordered list**

Unordered list is list that begins with a bullet point
(rather than characters that indicate order).

It is created with <*ul>* element.

Each item in the list is placed by using <*li>* element.

**Definition list**

Definition list mades up of a set of terms along with the definitions for each of those terms.
It list is created with the <*dl>* element.

<*dt>* is used to contain the term
being defined (the definition term).

<*dd>* is used to contain the definition.

**Nested list**

We can put a second list inside an <*li>* element to create a sublist or nested list.

![list in html](https://www.roseindia.net/tutorialfiles/31257.lists.jpg)

## Boxes

CSS treats each HTML element as if it lives in its own box.
We can set several properties that affect the appearance of these boxes.

**Boxes dimension**

By default a box is sized big enough to hold it's contents. To set our own dimensions for abox we can use the height and the width properties.

The most popular ways to specify the size of a box are to use pixels, percentages, or
ems.

pixels have been the most popular method
because they allow us to accurately control our size.

When we use the percentages, the size of the box is relative to the size of the browser window.

When we use ems, the size of the box is based on the size of text within it.

**Min-width & Max-width**

The *min-width* property specifies the smallest size a box can be displayed at when the browser
window is narrow.

The *max-width* property indicates
the maximum width a box can stretch to when the browser window is wide.

**Min-height & Max-height**

The *min-height* property defines the minimum height of an element.

The *max-height* property defines the maximum height of an element.

**Overflow**

The overflow property tells the browser what to do if the content contained within a box is larger
than the box itself.

**Hidden**

This property hides any extra content that does not fit in the box.

**Scroll**

This property adds a scrollbar to the box so that users can scroll to see the missing content.

**Border / Margin / Padding**

Every box has three available properties that
can be adjusted to control its appearance:
* Border
* Margin is a property controls the gap between boxes.
* Padding is the space between the border of a box and any content contained within it.

![box](https://sabe.io/classes/css/css-box-model-padding-border-margin/css-box-model.png)

The padding and margin properties
are very helpful in adding space between various
items on the page.

**Border**
The *border-width* property is used to control the width of a border.

We can control the style of a border using the *border-style* property like:
* solid
* dotted
* double
* dashed

Also we can use *border-color* to color the border.

If we want to center a box on the page (or center it inside the element that it sits in) we can set the left-margin and right-margin to auto.

The display property allows us to turn an inline element into a block-level element or vice versa, it is values are:
* inline
* block
* inline-block
* none

**Border images**
The *border-image* property applies an image to the border of any box.


The *box-shadow* property
allows you to add a drop shadow
around a box.

CSS3 introduces the ability to create rounded corners on any box, using a property called
*border-radius*.

### Basic JavaScript Instructions

**Arrays**
An array is a special type of variable, it stores a list of values.

Arrays are helpful when we do not know how
many items a list will contain.

We create an array by using let followed by the name of it.

![array](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/how-to-create-JavaScript-array.jpg)

*Array Literal*like this ( colors= ['white', 'black', 'custom']; )

*Array constructor* like this ( var colors=new Array('white ' , 'black', 'custom ' ); )

**VALUES IN ARRAYS**

Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).

We can change the value of an item an array by selecting it and assigning it a new value just as we would any other variable (using the equals sign and the new value for that item).

**Switch statement**

It is used to perform different actions based on different conditions.

A switch statement starts with a variable called the switch value.

Each case indicates a possible value for this variable and the code that should run if the
variable matches that value.

**How it works ?**

We have a default option that is run if
none of the cases match.

If a match is found, that code is run; then
the break statement stops the rest of
the switch statement running.

JavaScript can convert data types behind the scenes to complete an operation. This is
known as **type coercion**.

All values in JavaScript evaluate to either truthy or falsy.

JavaScript is said to use *weak typing* because the data type for a value can change.

Logical operators are processed left to right.
They short-circuit (stop) as soon as they have a
result, but they return the value that stopped
the processing.

**Loops**

It repeats something more than once. 
It checks a condition if it returns true, a code block will run then the condition will be checked again and if it still returns true the code block will run again until the condition returns false.

There are many types of loops like:
* For uses a counter as condition
* While
* Do while

A for loop is often used to loop
through the items in an array.

In while loop the loop will continue to run
for as long as the condition in the parentheses is true.

Do-while loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested:

![loop](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/JavaScript-Loop-Control.jpg)
