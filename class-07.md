# Domain Modeling
Domain modeling is the process of creating a conceptual model in code for a specific problem.

An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

Do not copy and paste. Writing out and testing our code will help us remember how to implement domain models in JavaScript later.

**Define a constructor and initialize properties**

To define the same properties between many objects, we'll want to use a constructor function.

The constructor function is defined using a function expression.

* The new keyword instantiates (i.e. creates) an object.

* The constructor function initializes properties inside that object using the this variable.

* The object is stored in a variable for later use.

**Generate random numbers**

To model the random nature of user behavior, we'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion.

methods can be added to a constructor function's prototype.

The percentage variable is assigned a decimal percentage based on the object's property.

Here's some tips to follow when building our own domain models:

1- When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.

2- Model its attributes with a constructor function that defines and initializes properties.

3- Model its behaviors with small methods that focus on doing one job well.

4-Create instances using the new keyword followed by a call to a constructor function.

5-Store the newly created object in a variable so we can access its properties and methods from outside.

6- Use the this variable within methods so we can access the object's properties and methods from inside.

## Tables

When representing information in a table, we need to think
in terms of a grid made up of rows and columns (a bit like a
spreadsheet).

A table represents information in a grid format.

The <*table>* element is used
to create a table. The contents
of the table are written out row
by row.

 <*tr>* stands for table row. It is followed by one or more
<*td>* elements (one for each cell
in that row).

The <*th>* element is used just
like the <*td>* element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)

The colspan attribute can be
used on a <*th>* or <*td>* element
and indicates how many columns
that cell should run across.

The rowspan attribute can be
used on a <*th>* or <*td>* element
to indicate how many rows a cell
should span down the table.

The headings of the table should
sit inside the <*thead>* element.

The body should sit inside the
<*tbody>* element.

The footer belongs inside the
<*tfoot>* element.

![tables](https://ictacademy.com.ng/wp-content/uploads/2017/10/HTML-Table-Structure.png)

### Functions, Methods, and Objects


The new keyword and the object  constructor create a blank object. We can then add properties and methods to the object .

To update the value of properties we use dot notation or square brackets.

They work on objects created using literal or constructor notation.

To delete property we use the delete keyword.

Object constructors can use a function as a template for creating objects.

![objects](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/How-to-Create-JavaScript-Objects.jpg)

The object is created on
the first line of the code sample. The properties and
methods are then added to it afterwards.

The function can be used to create multiple objects.
The this keyword is used instead of the object name.

The keyword this is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates.

When a function is defined inside an object, it
becomes a method.

In JavaScript, data is represented using name/value pairs.
To organize our data, we can use an array or object to group a set of
related values.

If we want to access items via a property name or key, use an object.

An object model is a group of objects, each of
which represent related things from the real world.
Together they form a model of something larger.

Web browsers implement objects that represent both
the browser window and the document loaded into the
browser window.

JavaScript also has several built-in objects such as
String, Number, Math, and Date. Their properties and
methods offer functionality that help you write scripts.

In JavaScript there are six data types:
Five of them are described as simple (or primitive) data types.
The sixth is the object (and is referred to as a complex data type).

The Math object has properties and methods
for mathematical constants and functions.
![ob](https://miro.medium.com/max/2722/1*iKJx57JU9sKdff-Os7upyA.png)
