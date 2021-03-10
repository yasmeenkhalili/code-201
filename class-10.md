# Error Handling & Debugging

**ORDER OF EXECUTION**

To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run.

**EXECUTION CONTEXTS**

The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.

Every statement in a script lives in one of three
execution contexts:
* GLOBAL CONTEXT
* FUNCTION CONTEXT
* EVAL CONTEXT (NOT SHOWN)

**The Stack** 

The JavaScript interpreter processes one line of code at a time .

When a statement has to call some other code in order to do its job the new task goes to the top of the pile of things to do.
Once the new task has been performed , the interpter can go back to the task in hand.

![stack](https://media.geeksforgeeks.org/wp-content/uploads/20190417203717/export-11.png)


Each time a script enters a new execution context, there are two phases
of activity: 
* PREPARE : 
   * The new scope is created
   * Variables, functions, and arguments are created
   * The value of the this keyword is determined
* EXECUTE :
   * Now it can assign values to variables
   * Reference functions and run their code
   * Execute statements

**UNDERSTANDING SCOPE**

In the interpreter, each execution context has its own variables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's variables object.

**UNDERSTANDING ERRORS**

If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code


**Error objects** can help us find where our mistakes are
and browsers have tools to help us read them.

When an Error object is created, it will contain the
following properties:
* name
* message
* file number
* line number


There are seven types of built-in error objects in
JavaScript:
* Error
* Syntax Error
* ReferenceError
* TypeError
* Range Error
* URIError
* EvalError

**HOW TO DEAL WITHERRORS**

There are two things we can do with the errors:

* DEBUG THE SCRIPT TO FIX ERRORS
* HANDLE ERRORS GRACEFULLY

## A DEBUGGING WORKFLOW

Debugging is about deduction: eliminating potential causes of an error.
* WHERE IS THE PROBLEM?
* WHAT EXACTLY IS THE PROBLEM?


The JavaScript console will tell us when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be.

The JavaScript console is just one of several developer tools that are
found in all modern browsers.

The console will show you when there is an
error in our JavaScript. It also displays the line
where it became a problem for the interpreter.

We can also just type code into the console
and it will show us a result.

Browsers that have a console have a console object, which has several
methods that our script can use to display data in the console.
The object is documented in the Console API.

The console.log() method
can write several values to the
console at the same t ime, each
separated by a comma,

**MORE CONSOLE METHODS**

1. console. info() can be used
for general information
2. console.warn() can be used
for warnings
3. console.error () can be used
to hold errors

If we want to write a set of
related data to the console, we
can use the console.group ()
method to group the messages
together.
When we have finished
writing out the results for the
group, to indicate the end of the
group the console .groupEnd ()
method is used.

console.table () method lets
us output a table showing:

* objects
* arrays that contain other
objects or arrays

Using the console.assert()
method, we can test if a
condition is met, and write to the
console only if the expression
evaluates to false.

**BREAKPOINTS**
We can pause the execution of a script on any
line using breakpoints. Then we can check the
values stored in variables at that point in time.

If we set multiple breakpoints, we can step
through them one-by-one to see where values
change and a problem might occur.


**CONDITIONAL
BREAKPOINTS**

We can indicate that a breakpoint should be
triggered only if a condition that we specify is
met. The condition can use existing variables


If we know our code might fail, use try, catch, and finally.
Each one is given its own code block.

**THROWING ERRORS**

If we know something might cause a problem for our script, we can
generate our own errors before the interpreter creates them.

To create our own error, we use the following line:

throw new Error( 'message'
);


**DEBUGGING TIPS**

* ANOTHER BROWSER
* ADD NUMBERS
* STRIP IT BACK
* SEARCH
* CODE PLAYGROUNDS
* VALIDATION TOOLS
* EXPLAINING THE CODE

![debugging](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/JavaScript-Debugging-and-Testing.png)