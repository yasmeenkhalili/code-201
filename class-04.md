# Links in HTML
Links allow us to move from one web page to another.
Links are created using the <*a>*
element which has an attribute
called href. The value of the
href attribute is the page that
we want people to go to when
they click on the link.

Writing a link as this 
<*a>* href =" url "Name</*a>*.

The value of the href attribute will be the full web address for the site, which is
known as an *absolute URL*.

When we are linking to other pages within the same site,
we do not need to specify the domain name in the URL. We can use a shorthand known as a
*relative URL*.

Folders on a website are sometimes referred to as directories.
The top-level folder is known
as the root folder.

The main homepage of a site
written in HTML (and the
homepages of each section in a
child folder) is called index.html.

URL is made up of the domain name
followed by the path to that page
or image.

**Relative URL Types**
* Same Folder : To link to a file in the same folder, just use the file
name. 
* Child Folder : For a child folder, use the name of the child folder, followed by a forward slash, then the file name.
* Grandchild Folder
Use the name of the child folder, followed by a
forward slash, then the name of the grandchild
folder, followed by another forward slash, then the file name.
* Parent Folder : Use ../ to indicate the folder above the current one, then follow it with the file name.
* GrandParent Folder
Repeat the ../ to indicate that we want to go up
two folders (rather than one), then follow it with the file name.

We use *target* if we want a link to open in a
new window,

*mailto* To create a link that starts up
the user's email program and
addresses an email to a specified
email address,

<*a href="#top">* links to the <*h1>* element at
the top of the page whose id
attribute has a value of top.

Ifwe want to link to a specific
part of a different page (whether
on our own site or a different
website) for example <*a href="http:/www.
htmlandcssbookcom/
#bottom">*.

We can use the id attribute to target elements within a page that can be linked to.

![link](https://i.pcmag.com/imagery/encyclopedia-terms/href-_href.fit_lim.size_1050x.gif)

## Layout

**Building Blocks**

CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
Block-level boxes start on a new line and act as the main building blocks of any layout,while inline boxes flow between surrounding text.

To separate boxes, we can use
borders, margins, padding, and background colors.

If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.

CSS has the following positioning schemes that allow us to control the layout of a page: normal flow, relative positioning, and absolute
positioning.

We can float elements using the float property.

To indicate where a box should be positioned, we need to use box offset properties to tell the browser how far from the top or bottom
and left or right it should be placed.

**Normal flow**
( position:static )
In normal flow, each block-level
element sits on top of the next
one.

**Relative positioning** ( position:relative )
moves an element in relation to where it
would have been in normal flow.


**Absolute Positioning** ( position:absolute )
When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page.

**Fixed Positioning** ( position:fixed ) is a type
of absolute positioning that
requires the position property
to have a value of fixed.

**Floating Elements** ( float ) is a property allows us
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.

The following three CSS
properties are used to position
the columns next to each other:
* width
this sets the width of the
columns.
* float
this positions the columns next
to each other.
* margin
this creates a gap between the
columns.

We should take care of this during coding
:

* **Screen Sizing**
our design needs to be able to
work on a range of different sized screens

* **Screen Resolution**
Resolution refers to the number of dots a screen shows per inch

* **Page Sizes**
web
designers often try to create pages of around 960-1000 pixels wide

* **Fixed Width Layouts**
Measurements tend
to be given in pixels.
* **Liquid Layouts**
Liquid layout designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages.

Many designers use a **grid structure** to help them
position items on a page, and the same is true for web designers

![grid](https://i2.wp.com/gridexamples.com/wp-content/uploads/2018/02/CSSgrid-examples.jpg?fit=800%2C402&quality=100&strip=all&ssl=1)



The **960_12_col.css stylesheet**
contains all of the rules we need
to control the grid layout. The
HTML uses the class names.

![960grid](https://i.pinimg.com/originals/95/25/28/952528657256a280028ebb2a8a17a10f.jpg)


### Function

It groups a series of statements together to perform a
specific task.

The name of functions should describe the task it is performing.

function is executed when "something" invokes it (calls it).

function is defined with the function keyword, followed by a name, followed by parentheses ().

Some functions have a return value.

Sometimes a function needs specific information to perform it's task.

![function](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2019/03/JavaScript-function-tutorial.jpg)

A function declaration creates a function that you
can ca ll later in your code.

A function with no name is called an anonymous
function.

**Variable scope**

The location where we declare a variable will affect where it can be used
within our code. If we declare it within a function, it can only be used
within that function. This is known as the variable's scope.

When a variable is created inside a function using the
var keyword, it can only be used in that function.
It is called a local variable.

If we create a variable outside of a function, then it
can be used anywhere within the script. It is called a
global variable.
![variable](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/JavaScript-Variables-1200x675.png)


**Article**
To improve the quality of code developers produce these are some of practices: 
 * produceIterative loops
 * Code reviews
 * Fast feedback. 
 * Error checking 
 * linting

 **Pair programming** commonly involves two roles: the Driver and the Navigator.


  The Driver is the programmer who manages the text editor, switching files, version control, and writing—code.

  The Navigator uses their words to guide the Driver , thinks about the big picture, what comes next, how an algorithm might be converted in to code.

  There are four fundamental skills that help anyone learn a new language:
   * Listening: hearing and interpreting the vocabulary 
   * Speaking: using the correct words to communicate an idea 
   * Reading: understanding what written language intends to convey 
   * Writing: producing from scratch a meaningful

Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging.

Researches also identified pairing enhances technical skills, team communication, and even enjoyability of coding in the workplace.

**Benifits from  pair program**

* Greater efficiency
* Engaged collaboration
* Learning from fellow students
* Social skills
* Job interview readiness
* Work environment readiness


