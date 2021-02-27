# Introductory HTML and JavaScript

**How websites are created ?**

Small websites are written using *HTML* & *CSS*.
By the time HTML & CSS are improved and now there are many versions of them, the latest versions are **HTML5** & **CSS3**.

Some sites are very complex so may use a database to store data, and programming languages such as PHP, ASP, Net, Java.

**How the web works ?**

 First we should know some concepts.
 * People access websites using
software called a **web browser** like *Chrome* and *Firefox*.

* When we ask our browser for a web page, the request is sent across the Internet to a special
computer known as a **web server** which hosts the website.

* To find the location of the web server, our browser will first connect to a **Domain Name System (DNS)** server, that tell our browser how to find the website. 

So we enter the web address that we want to access it on our browser , the computer contacts the network of srevers (DSN) that returns the IP address associated with the web that we want to access it . This IP allows our browser to contact the web server that hosts the website we requested.The web server then sends the page we requested back to our web browser.

![How web works?](https://cdn.business2community.com/wp-content/uploads/2021/01/DNS-Diagram.png)


## HTML 
**How Pages Use Structure**

Structure helps users to understand the web page.
Such as what is the heading , where is the end of the page ... .

HTML Describes the Structure of Pages.To
describe the structure of a web page, we add code to the words we want to appear on the page.

The HTML code is made up of characters that live inside angled brackets — these are called *HTML elements* that are using to describe the structure of pages.
Each element has open and closing tag that act as container as we see in the image: 

![Html element](https://cdo-curriculum.s3.amazonaws.com/media/uploads/html_element.png)

**Attribute**

Attributes provide additional information
about the contents of an element.They appear
on the opening tag of the element and are
made up of two parts: a name and a value,
separated by an equals sign.

![Attribute](https://lh3.googleusercontent.com/proxy/-nBTAAiYqvKNlzlK684G0aPtdx-Igu89EY_y_brkIwJgXVhAOwbZZBo7UBKpl8otFBeV6feo3cMI0gkoCngsGVC_rKTeZq6vTgHh0aQNOGf05MFD6a7RjjQhR0yJoGuPQJoldraDGmyiWtUlbXJcYM_5dSWI0kNdH8q4-Gb4)

When we write a code in html we are dealing with basic elements like body, head, title .

In the *body* element everything inside it is shown inside the main browser window.

*Head* element contains information about the page and usually find *title* element inside it.

![Elements](https://miro.medium.com/max/498/1*5gJzummAqpBDGATo0fjU6Q.jpeg)

**Extra markup**

Since the web was first created, there have
been several different versions of HTML.Each new version was designed to be an improvement on the previous one.
* HTML4 Released 1997
* XHTML 1.0 Released 2000
* HTML5 Released 2000

Because there have been several versions of HTML, each web page should begin with a **DOCTYPE** declaration to tell a browser which version of HTML the page is using.

Here is some of useful elements : 

* *<*!-- comment goes here --> we can add any comment to our code and it will not be visible in the user's browser.
* id attribute it is used to uniquely identify that element from other elements on the page.

* Class attribute is used to identify several elements as being different from the other elements on the page.

* Some elements will always
appear to start on a new line in
the browser window. These are
known as **block level** elements like <*h1>* <*p>* <*ul>* and <*li>*.

* Some elements will always appear to continue on the same line as their neighbouring elements. These are known as **inline elements** like <*a>* <*b>* <*em>* and <*img>*.

* The <*div>* element allows us to group a set of elements together in one block-level box.

* The <*meta>* element lives inside the <*head>* element and contains information about that web page.

**Escape Characters** are used to include special
characters in our pages such as <, >, and ©.


**HTML5 Layout**

It is introducing a new set of elements that help define the structure of a page.
Like the <*header>* and <*footer>* elements.
 
Some of HTML5 elements :

* The *header* appears at the top of the page and may used to contain the site name and the main navigationthe.

* The *footer* appears at the bottom of the page and may contains  copyright information, along with links to the privacy policy and terms and conditions.

* The <*nav>* element is used to contain the major navigational blocks on the site.

* The <*article>* element acts as a container for any section of a page that could stand alone and
potentially be syndicated.

* The <*section>* element groups related content together, and typically each section would have its own heading.

* The purpose of the <*hgroup>* element is to group together a set of one or more <*h1>* through
<*h6>* elements so that they are treated as one single heading.

* <*figure>* and <*figcaption>* elements to contain an image.

**Process & Design**

When we are going to create a website we should ask ourself some questions before :

* Who is the site for ?
* Why people visit our website ?
* What our visitors are trying to achieve ?
* What information our visitors need ?
* How often people will visit our site ?

**Site Maps** the aim from it is to create a diagram of the pages that will be used to structure the site. Like this image:

![site map](https://i.pinimg.com/originals/1c/c5/f4/1cc5f4ec000969f11eedf4dbe0f8c9d8.png)


**A wireframe** is a simple sketch of the key
information that needs to go on each page of a
site. Like this : 

![wireframe](https://www.ibm.com/support/knowledgecenter/SSYMRC_6.0.6/com.ibm.rational.rrm.help.doc/images/wireframe_1.gif)

*Visual hierarchy* helps visitors understand what we are trying to tell them.

We can differentiate between pieces of information using size, color, and style.


### JavaScript 

JavaScribt allows to us to make our web pages more interactive by accessing and modifying the content.

In simple language JS:
* Access the content of the page
* Modify the content of the page
* Program rules or instructions the browser can follow
* React to events triggered by the user or browser

**The ABC of Programming**

There is some of key concepts in computer programming one of them is **Script**.

Script is a series of introductions that a computer can follow to achieve a goal.
To write it we should specify our goal and then list the tasks that need to be completed in
order to achieve it.

So to begin programming we should do these steps:

* Define the goal
* design the script
* Code each step

To start coding we must deal with this:

* Vocabulary: The words that computers understand
* Syntax: How you put those words together to
create instructions computers can follow.

Computers create models of the world using *data*.
In computer programming, each physical thing in
the world can be represented as an *object*. Each object has specialist features the programmer called it *properties* of an object.
Each property has a name and a value.

programs are designed to do different things when users interact with the computer in different ways.The code for a method can contain lots of
instructions that together represent one task.

Finally when we put all above together:
Computers use data to create models of things in the real world.
The events, methods, and properties of an object all relate to each other:
Events can trigger methods, and methods can retrieve or update an object's properties.

**How a browser sees a web page**
* Receive a page as HTML code
* Create a model of the page and store it in the memory 
* Use a rendering engine to show the page on the screen

**Creating a basic JavaScript**

* JavaScript is written in plain text and it has .js file extension.
* When we want to use JavaScript with a web page, we use the HTML <*script>* element to tell the browser it is coming across a script. We put it at the end of the body tag. The <*link>* element can be used to load a CSS file.

And as we see in this image we start creating our website by writing Html file and style it using Css and finally make it interactive by using JavaScript.

![HTML CSS JS](https://miro.medium.com/max/3060/1*HHzwtxH4HYE57TmTAA4CPA.png) 






