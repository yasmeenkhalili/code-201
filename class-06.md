# The problem Domain

What is the hardest thing about writing code?

* Learning a new technology
* Naming things
* Testing the code
* Debugging
* Fixing bugs
* Making software maintainable

Understanding the *Problem Domain* is the hardest part of programming.

In writing code we put together code with the purpose of building components of the problem domain.

Programming is easy if we understand the problem domain.

If understanding the problem domain is the hardest part of programming and we want to make programming easier, we can do one of two things:

* Make the problem domain easier
* Get better at understanding the problem domain

We can often make the problem domain easier by cutting out cases and narrowing our focus to a particular part of the problem.
This means ,take a part of the problem and fully understand that part before expanding the problem domain.


**Simple set of steps** to follow which we can use for any algorithm type programming problem:
* Read the problem completely twice.
* Solve the problem manually with 3 sets of sample data.
* Optimize the manual steps.
* Write the manual steps as comments or pseudo-code.
* Replace the comments or pseudo-code with real code.
* Optimize the real code.

![problem domain](https://texavi.co.uk/insights/posters/Texavi_Poster_BusinessAnalysis_ProblemvsSolution.png)

## What is an object ?

Objects group together a set of variables and functions to create a model of a something we would recognize from the real world. In an object,
variables and functions take on new names.

In an object : variables become known as properties and is called *property*.

In an object : functions become known as properties and is called *method*.

An object can not have two keys
with the same name.

The value of a property can be a
string, number, Boolean, array, or
even another object. The value of a
method is always a function.

**Creating an object**

There is various way to create an object in JavaScript.

![object](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/How-to-Create-JavaScript-Objects-1200x675.jpg)

We can access the properties or methods of an object using dot notation.
And we can access properties using square brackets.

### Document Object Model (DOM)

The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.

It covers two primary areas:
* Making a model of the HTML page
The DOM specifies the way in which the
browser should structure this model using
a *DOM tree*.

* Accessing and changing the Html page

As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.

It consists of four main types of nodes:
* THE DOCUMENT NODE
* ELEMENT NODES
* ATTRIBUTE NODES
* TEXT NODES
![dom](https://snipcademy.com/img/articles/javascript-document-object-model/dom.svg)


Accessing and updating the DOM tree involves two steps:

* Locate the node that represents the element you want to work with.
* Use its text content, child elements, and attributes.

**ACCESS THE ELEMENTS**

* SELECT AN INDIVIDUAL

   * ELEMENT NODE : get ElementByld()
Uses the value of an element's
id attribute
  * querySelector()

* SELECT MULTIPLE
ELEMENTS (NODELISTS)
  * getElementsByClassName()
  * getElementsByTagName()
  * querySelectorAll()

* TRAVERSING BETWEEN
ELEMENT NODES
  * parentNode
  * previousSibling / nextSibling
  * firstChild / lastChild

**WORK WITH THOSE ELEMENTS**

* ACCESS/ UPDATE
TEXT NODES
* WORK WITH HTML
CONTENT 
   * innerHTML
   * textContent
   * create Element(): Create the element
   * createTextNode() : Give it content
   * appendChild() / removeChild() : Add it to the DOM or remove it 

* ACCESS OR UPDATE ATTRIBUTE VALUES

   * className /id
   * hasAttribute()
   * getAttribute()
   * setAttribute()
   * removeAttribute()



DOM queries may return one element, or they may return a Nodelist,
which is a collection of nodes.

If a method can return more than one node, it will
always return a Nodelist, which is a collection of
nodes.


There are two ways to select an element from a Nodelist:
The item() method and array syntax.
Both require the index number of the element we want.


When we have an element node, we can select
another element in relation to it using these five
properties. This is known as traversing the DOM.
* parentNode : This property finds the element
node for the containing (or
parent) element in the HTML.
* previousSibling
nextSibling : 
These properties find the
previous or next sibling of a node
if there are siblings.
* firstChild / 
lastChild : These properties find the first or
last child of the current element.

The document object's write () method is a simple
way to add content that was not in the original
source code to the page, but its use is rarely advised.

The innerHTML property lets you get/update the
entire content of any element (including markup) as a string.

DOM manipulation refers to using a set of methods
and properties to access, create, and update
elements and text nodes.


**VALIDATE INPUT GOING TO THE SERVER**

**XSS**

![browser](https://static.packt-cdn.com/products/9781788394185/graphics/bed80c21-f2a3-4fb4-8e26-c4ddd1243466.png)

Make sure that our users can only input characters they need to use
and limit where this content will be shown on the page.

Any content generated by users that contain characters that are used
in code should be escaped on the server. We must control any markup
added to the page.


The hasAttribute() method
of any element node lets us
check if an attribute exists.

The setAttribute() method
allows us to update the value
of any attribute.

To remove an attribute from an
element, first select the element,
then call removeAttribute().

![xss](https://media.geeksforgeeks.org/wp-content/uploads/20190516152959/Cross-Site-ScriptingXSS.png)






