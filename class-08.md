# Layout

**Controlling the position of elements**

CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.

* Block-level elements
start on a new line
Examples include:
<*h1>* <*p>* <*ul>* <*li>*
* Inline elements
flow in between
surrounding text
Examples include:
<*img>* <*b>* <*i>*

**Containing Elements**
If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.

CSS has the following positioning schemes that allow us to control
the layout of a page: 
* normal positioning : Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
* relative positioning: This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed.
* absolute positioning: This positions the element
in relation to its containing
element. It is taken out of
normal flow.

To indicate where a box should be positioned, we may also need to use
box offset properties to tell the browser how far from the top or bottom
and left or right it should be placed:

* Fixed Positioning
* Floating Elements

When we move
any element from
normal flow, boxes
can overlap. The
z-index property
allows us to control
which box appears
on top.

**float**  allows us
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.

A lot of layouts place boxes
next to each other. The float
property is commonly used to
achieve this.


![position](https://i.pinimg.com/736x/ab/36/1d/ab361d33a7fccd7f2958b3963ce1c302.jpg)
 **clear** allows us
to say that no element (within
the same containing element)
should touch the left or righthand
sides of a box.

Many web pages use multiple
columns in their design. This
is achieved by using a <*div>*
element to represent each
column.
* width : This sets the width of the
columns.
* float : This positions the columns next
to each other.
* margin : 
This creates a gap between the
columns.

**Screen Sizes**

Different visitors to your site will have different sized screens that show
different amounts of information, so our design needs to be able to
work on a range of different sized screens.

**Screen Resolution**

Resolution refers to the number of dots a screen shows per inch.

**Page Sizes**
Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide.

**Fixed width layout**
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.

**Liquid layout** designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages.

**Layout Grids**
to show you how the
page was designed according to
a grid. This grid is called the 960
pixel grid and is widely used by
web designers.

Grids set consistent proportions
and spaces between items which
helps to create a professional
looking design.

* Creates a continuity between
different pages which may
use different designs
* Helps users predict where to
find information on various
pages
* Makes it easier to add new
content to the site in a
consistent way
* Helps people collaborate
on the design of a site in a
consistent way

![layout grid](https://miro.medium.com/max/1024/1*XCZZZmhQN4rHLw2dW14BZQ.png)

**CSS frameworks** aim to make our life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on.

**The 960_12_col.css** stylesheet contains all of the rules we need to control the grid layout. The HTML uses the class names.

![grid](https://mac-cdn.softpedia.com/screenshots/960-grid-system-overlay-unofficial_1.jpg)