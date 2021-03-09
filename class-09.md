# Forms
The term 'form' has referred
to a printed document that contains
spaces for us to fill in information.

HTML borrows the concept of a form to refer to different
elements that allow us to collect information from visitors to
our site.

The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage it is
enabling users to
search, forms also allow users
to perform other functions
online.

**Form Controls**

There are several types of form controls:
* ADDING TEXT
* Making Choices
* Submitting Forms
* Uploading Files

**How Forms Work ?**

A user fills in a form and then presses a button
to submit the information to the server.

![form](https://slideplayer.com/slide/6232568/20/images/4/Collecting+Data+with+Forms.jpg
)

**Form Structure**

* Form controls live inside a
<*form>* element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.
* Every <*form>* element requires
an action attribute. Its value
is the URL for the page on the
server that will receive the
information in the form when it
is submitted.
* Forms can be sent using one of
two methods: get or post.

The <*input>* element is used
to create several different form
controls.

**Text Input**

type="text"
When the type attribute has a
value of text, it creates a singleline
text input.

**Password Input**

type="password"
When the type attribute has
a value of password it creates
a text box that acts just like a
single-line text input, except
the characters are blocked out.

**Text Area**

The <*textarea>* element
is used to create a mutli-line
text input. Unlike other input
elements this is not an empty
element.

**Radio Button**

type="radio"
Radio buttons allow users to pick
just one of a number of options.

**Checkbox**

type="checkbox"
Checkboxes allow users to select
(and unselect) one or more
options in answer to a question.

**Drop Down List Box**

A drop down list box (also
known as a select box) allows
users to select one option from a
drop down list. 

**File Input Box**

This type of input creates a
box that looks like a text input
followed by a browse button to allow users to
upload a file.

**Submit Button**

type="submit"
The submit button is used to
send a form to the server.

**Image Button**

type="image"
If we want to use an image for
the submit button, we can give
the type attribute a value of
image.

The <*button>* element was
introduced to allow users more
control over how their buttons
appear, and to allow other
elements to appear inside the
button.

We can group related form
controls together inside the
<*fieldset>* element.

We have seen forms
on the web that give users
messages if the form control has not been filled in correctly; this is
known as **form validation**.

## HTML5
HTML5 is introducing validation and
leaving the work to the browser.
Validation helps ensure the
user enters information in a
form that the server will be able
to understand when the form
is submitted.

HTML5 introduces new form
controls to standardize the
way that some information is
gathered.

HTML5 has also introduced
inputs that allow visitors to
enter email addresses and URLs.
Browsers that do not support
these input types will just treat
them as text boxes.

If we want to create a single
line text box for search queries,
HTML5 provides a special type
of input for that purpose.

![html5](https://lh3.googleusercontent.com/proxy/sKTHkzroQH9MQwUvaWhYTl1f7Xz_jOeB9bWyIKNuGhWQyHHfigtFLEwVBLJ-Gz4EvV5lvR8ygvrZhZ_v_lkuqjVKC_4je_yx39ALeZ5kpVssthGyAakbTA)


### Lists, Tables and Forms

The **list-style-type** property
allows us to control the shape
or style of a bullet point (also
known as a marker).
It can be used on rules that
apply to the <*ol>*, <*ul>*, and <*li>*
elements.

**Unordered Lists**

For an unordered list we can use
the following values:
* none
* disc
* circle
* square

We can specify an image to act
as a bullet point using the
**list-style-image** property.
This property can be used on
rules that apply to the <*ul>* and
<*li>* elements.

Lists are indented into the page
by default and the **list-style-position**
property indicates
whether the marker should
appear on the inside or the
outside of the box containing the
main points.

**Table Properties**
* width to set the width of the
table
* padding to set the space
between the border of each table
cell and its content
* text-transform to convert the
content of the table headers to
uppercase
* letter-spacing, font-size
to add additional styling to the
content of the table headers
* background-color to change
the background color of the
alternating table rows


If we have empty cells in
our table, then we can use
the empty-cells property to
specify whether or not their
borders should be shown.

It can take one of three values:
* show
* hide
* inherit

**collapse**
Borders are collapsed into a
single border where possible.
(border-spacing will be
ignored and cells pushed
together, and empty-cells
properties will be ignored.)


## Events

Events are "things" that happen to HTML elements.

Here is a selection of the events that occur in the browser while we are
browsing the web:
* UI EVENTS
  * load
  * unload
  * error
  * resize
  * scroll
* KEYBOARD EVENTS
  * keydown
  * keyup
  * keypress
* MOUSE EVENTS
   * click
   * dblclick
   * mousedown
   * mouseup
   * mousemove
   * mouseover
   * mouseout

When an event has occurred, it is often described as having **fired** or
been **raised**.
 
Events are said to trigger a function or script.

**FOCUS EVENTS**

Occur when an element (e.g., a link or form field) gains or loses focus
* focus / focusin
* blur / focusout

**FORM EVENTS**

Occur when a user interacts with a form element
* input
* change
* submit
* reset
* cut
* copy
* paste
* select

**MUTATION EVENTS**
Occur when the DOM structure has been changed by a script
.To be replaced by mutation observers
* DOMSubtreeModified
* DOMNodelnserted
* DOMNodeRemoved
* DOMNodelnsertedlntoDocument
* DOMNodeRemovedFromOocument


When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code.
Together these steps are known as event handling.
* **SELECT ELEMENT** 
Select the element
node(s) we want the
script to respond to.
* **SPECIFY EVENT**

Indicate which event on
the selected node(s) will
trigger the response.
* **CALL CODE**

State the code we want
to run when the event
occurs.

![event](https://images.slideplayer.com/31/9755584/slides/slide_2.jpg)

### THREE WAYS TO BIND AN EVENT TO AN ELEMENT

* HTML EVENT
HANDLERS
The value of the event handler
attributes would be JavaScript
* TRADITIONAL DOM
EVENT HANDLERS
* DOM LEVEL 2 EVENT
LISTENERS

![pind](https://image.slidesharecdn.com/qew2fe1qfouq3ez0irrw-signature-a5e16f8a5f9bf5c06bfd992151090953475efa37da75f9eed6674474188d6d90-poli-141218052940-conversion-gate02/95/angular-js-10-638.jpg?cb=1418892818)

**Event listeners** are a more recent approach to handling events.
They can deal with more than one function at a time
but they are not supported in older browsers.

![liste](https://miro.medium.com/max/452/1*6z7TmtoXux9NZ3U9LfeQnw.jpeg)

## Event Flow
HTML elements nest inside other elements.
![event bubbling](https://static.javatpoint.com/javascriptpages/images/event-bubbling-and-capturing-in-javascript6.png)


The flow matters when our code has event handlers and on an element or and one of it's ancestor or descendant elements.


When an event occurs, the event object tells
us information about the event, and the
element it happened upon.


**EVENT DELEGATION**

Creating event listeners for a lot of elements
can slow down a page, but event flow allows
us to listen for an event on a parent element.

BENEFITS OF EVENT DELEGATION
* WORKS WITH NEW
ELEMENTS
* SOLVES LIMITATIONS
WITH this KEYWORD
* SIMPLIFIES OUR
CODE

**CHANGING DEFAULT
BEHAVIOR**
The event object has methods that change:
the default behavior of an element and how
the element's ancestors respond to the event.

* preventDefault ()
* stopPropagation()
* USING BOTH METHODS

When calling a function, the event object's target property is the best
way to determine which element the event occurred on.

The *this KEYWORD*
The this keyword refers to the
owner of a function. On the right,
this refers to the element that
the event is on.

The HTML elements we can interact with, such as links and form
elements, can gain focus. These events fire when they gain or lose focus.

## Where events occur

The event object can tell us where the cursor saw positioned when an event was triggered.

Whenever elements are added to or removed from the DOM, its
structure changes. This change triggers a mutation event

The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.