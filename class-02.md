# Text in HTML
As we Know to create web page we should add tags to the contents of the page, this called *markup*.

**Headings**

HTML has 6 levels of headings from h1 (main heading), h2 (subheading) upto h6.
They are different in size and in the importance of the content.

**Paragraph**

To create a paragraph, surround the words that make up the paragraph with an opening <*p>*
tag and closing <*/p>* tag.

We can style any text in heading or in paragraph by using :
* <*b>* for **Bold**
* <*i>* for *Italic*
* The <*sub>* element is used to contain characters that should be subscript such as using in chemical formulas.
* <*br />* to make line break.
* <*hr/>* to add a horizontal rule between sections.

**HTML editors**

Like *visual studio code* usually have two views of the page that we are creating:
 * a visual editor : displays the content (text) in an easy to look at and good view.
 * a code view : where we can see and edit the code.
 
 **Semantic markup**

It describes the element meaning to the browser and the developer, like
* <*strong>* tells that content has strong importance.
* <*blockquote>* used for longer quotes that take
up an entire paragraph.
* <*address>* use to contain contact details for the author of the page.

## Introducing CSS

CSS (cascading style sheets) give the rule to style the HTML contents and makes them more attractive.
A CSS rule contains two parts: a selector and a declaration. 

![Css rule](https://www.w3schools.com/css/selector.gif)

**Types of CSS**
* Inline 
* Internal: put the css rules iside <*style>* element that usually sites inside <*head>* element
* External: create a file with .css extesion and put the css rules inside it then link this file with html file using <*link>* element that sites inside <*head>* element 

![Css type](https://www.bitdegree.org/learn/storage/media/images/8c4493d3-110c-4a95-8b70-7626ce2d2f4e.jpg)


**CSS Selectors**
It is patterns used to select the element(s) we want to style.
Some of these selectors:
* Universal Selector * 
* Type Selector h1, h2, h3 
* Class Selector .
* ID Selector #


**How Css Rules Cascade**
If there are two or more rules that apply to the same element, it is important to understand
which will take precedence, it depends on mant things :
* Last rule
* Importance
* Specificity


**Why use External Style Sheets ?**

The benefits from using External style sheets are:
* All web pages can style the same by using link element, that means we dont need to repeat the code every page.
* The site will load faster
* Easy to Change the CSS rules 

### Basic JavaScript Instructions
As we know before a script is a series of instructions that a computer can follow one-by-one.
Each step called **statment** that should end with a semicolon.
The semicolon also tells the JavaScript interpreter when a step is over, indicating that it should move to the next step.

Some statements are surrounded by curly braces;
these are known as *code blocks*

JAVASCRIPT is case sensitive, so we should be careful during coding.

We can add a single line comment by starting the line with // and for multi-line comments starting the comments with the /* characters and ending with the */ characters.

**Variable** 

It is something like container with dynamic value that can be changed dynamically.
Before using variable we should declare it (give it name) like this *var quantity;*

**Data Types**
* Number like (var price=10;)
* String like (var Name='SUN';)
* Boolean true or false like (var inStock=false;)

**Rules for naming variable**
* The name must begin with a letter, dollar sign ($),or an underscore (_).
* The name can contain letters, numbers, dollar sign ($), or an underscore (_).
* We cannot use keywords or reserved words.
* All variables are case sensitive.
* Use a name that describes the kind of information that the variable stores.
* Use a capital letter for the first letter of
every word after the first word when the variable has more than word.

**Arrays**

An array is a special type of variable. It doesn't
just store one value; it stores a list of values.

It is helpful when we do not know how
many items a list will contain.

![arrays type](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/how-to-create-JavaScript-array.jpg)

**Array Literal** like this ( colors= ['white',
'black',
'custom']; )

**Array constructor** like this ( var colors=new Array('white ' ,
'black',
'custom ' ); )

**VALUES IN ARRAYS**

Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one).

We can change the value of an item an array by selecting it and assigning it a new value just as
we would any other variable (using the equals sign and the new value for that item).

**EXPRESSIONS**
It is evaluating into a single value.

Type of expressions 

* That just assign a value to a variable, like this var color = 'beige';
* That use two or more values to return a single value, like this var area = 3 * 2;

**OPERATORS**

They allow programmers to create a single value from one or more values.

* Assignment operators ( color = 'beige'; )
* Comparison operators (buy = 3 > 5;)
* Arithmetic operators (area = 3 * 2;)
* String operators (greeting= 'Hi'+ 'Molly';)
* Logical operators (buy= (5 > 3) && (2 < 4);)


#### Decisions and Loops


**Decision Making**
Flowcharts can help us plan for which lines of code should be run next.
There are 2 components to a decision :
* An expression is evaluated , which return a value
* A conditional statement says what to do in a given situation

We evaluate a situation by comparing one value in the script to what we expect it might to be.
The result will be a Boolean (true or false).

![Comparison operator](https://i.ytimg.com/vi/wFB-ywsNPwg/maxresdefault.jpg)

![logical operator](https://chunxuchai.files.wordpress.com/2019/05/logical-operator.jpg)

**IF statement**

If statement evaluates or check the condition. If the condition is true , any statements in the subsequent code block are excuted.

**The IF ... else statement**

It checks a condition if it is true , the first code block is excuted . If the condition is false , the second code block is run instead.

![if else statement](https://cdn.javascripttutorial.net/wp-content/uploads/2016/08/JavaScript-if-else-statment.png)






