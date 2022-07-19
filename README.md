[![Pixel To Code GitHub Banner](https://github.com/pixel2code/pixel2code/raw/main/GitHubHeader.png)](https://pixeltocode.co)

# JavaScript For Beginners

[Introduction to JavaScript](#introduction-to-javascript) | 
[History](#history) | 
[Just JavaScript](#just-javascript) | 


---

## [Introduction](https://pixeltocode.co)

Welcome to the official Pixel To Code JavaScript For Beginners.
This project does not try to cover everything under the sun related to javaScript. 
It focuses on the core of the language, trying to simplify the more complex topics.
I hope the contents of this project will help you achieve what you want: ```Learn the basics of JavaScript```

<h2 id="introduction-to-javascript">Introduction to JavaScript</h2>

JavaScript is one of the most popular programming languages in the world. 
I believe it's a great language to be your first programming language ever. 
We mainly use JavaScript to create
-   Websites
-   Web applications
-   Server-Side Applications using Node.js

but JavaScript is not limited to these things, and it can also be used to
-   Create mobile applications using tools like React Native 
-   Create programs for micro controllers and the internet of things 
-   Create smartwatch applications


It can basically do anything. It's so popular that everything new that shows up is going to have some kind of JavaScript integration at some point.

JavaScript is a programming language that is:

- ***High level***: it provides abstractions that allow you to ignore the details of the machine where it's running on. 
It manages memory automatically with a garbage collector, so you can focus on the code instead of managing memory like other languages like C would need, and provides many constructs which allow you to deal with highly powerful variables and objects.

- ***Dynamic***: opposed to static programming languages, a dynamic language executes at runtime many of the things that a static language does at compile time. 
This has pros and cons, and it gives us powerful features like dynamic typing, late binding, reflection, functional programming, object runtime alteration, closures and much more. 
Don't worry if those things are unknown to you - you'll know all of those at the end of the project.

- ***Dynamically typed***: a variable does not enforce a type. You can reassign any type to a variable, for example, assigning an integer to a variable that holds a string.

- ***Loosely typed***: as opposed to strong typing, loosely (or weakly) typed languages do not enforce the type of an object, allowing more flexibility but denying us type safety and type checking (something that TypeScript - which builds on top of JavaScript - provides)

- ***Interpreted***: It is commonly known as an interpreted language, which means that it does not need a compilation stage before a program can run, as opposed to C, Java or Go for example. In practice, browsers do compile JavaScript before executing it, for performance reasons, but this is transparent to you: there is no additional step involved.

- ***Multi-paradigm***: the language does not enforce any particular programming paradigm, unlike Java for example, which forces the use of object-oriented programming, or C that forces imperative programming. You can write JavaScript using an object-oriented paradigm, using prototypes and the new (as of ES6) classes syntax. You can write JavaScript in a functional programming style, with its first-class functions, or even in an imperative style (C-like).

In case you're wondering, JavaScript has nothing to do with Java, it's a poor name choice but we have to live with it.

<h2 id="history">History</h2>

Created in 1995, JavaScript has gone a very long way since its humble beginnings.

It was the first scripting language that was supported natively by web browsers, and thanks to this it gained a competitive advantage over any other language and today it's still the only scripting language that we can use to build Web Applications.

Other languages exist, but all must compile to JavaScript - or more recently to WebAssembly, but this is another story.

In the beginnings, JavaScript was not nearly powerful as it is today, and it was mainly used for fancy animations and the marvel known at the time as Dynamic HTML.

With the growing needs that the web platform demanded (and continues to demand), JavaScript had the responsibility to grow as well, to accommodate the needs of one of the most widely used ecosystems of the world.

JavaScript is now widely used also outside of the browser. The rise of Node.js in the last few years unlocked backend development, once the domain of Java, Ruby, Python, PHP and more traditional server-side languages.

JavaScript is now also the language powering databases and many more applications, and it's even possible to develop embedded applications, mobile apps, TV sets apps and much more. What started as a tiny language inside the browser is now the most popular language in the world.

<h2 id="just-javascript">Just JavaScript</h2>

Sometimes it's hard to separate JavaScript from the features of the environment it is used in.

For example, the ```console.log()``` line you can find in many code examples is not JavaScript. Instead, it's part of the vast library of APIs provided to us in the browser. In the same way, on the server it can be sometimes hard to separate the JavaScript language features from the APIs provided by Node.js.

Is a particular feature provided by React or Vue? Or is it "plain JavaScript", or "vanilla JavaScript" as often called?

In this project I talk about JavaScript, the language.

Without complicating your learning process with things that are outside of it, and provided by external ecosystems.

<h2 id="syntax">Syntax</h2>

In this little introduction I want to tell you about 5 concepts:
- white space 
- case sensitivity 
- literals 
- identifiers 
- comments

###White space

JavaScript does not consider white space meaningful. Spaces and line breaks can be added in any fashion you might like, even though this is in theory.

In practice, you will most likely keep a well defined style and adhere to what people commonly use, and enforce this using a linter or a style tool such as Prettier.

For example, I like to always have 2 characters to indent.

### Case sensitive

JavaScript is case sensitive. A variable named ```something``` is different from ```Something``` .
The same goes for any identifier.

### Literals

We define as ***literal*** a value that is written in the source code, for example, a number, a string, a boolean or also more advanced constructs, like Object Literals or Array Literals:

```
5
'Test'
true
['a', 'b']
{ color: 'red', shape: 'Rectangle'}
```

### Identifiers

An ***identifier*** is a sequence of characters that can be used to identify a variable, a function, an object. It can start with a letter, the dollar sign $ or an underscore ```_``` , and it can contain digits. Using Unicode, a letter can be any allowed char, for example, an emoji 😄.

```
Test
test
TEST
_test
Test1
$test
```

The dollar sign is commonly used to reference DOM elements.
Some names are reserved for JavaScript internal use, and we can't use them as identifiers.

### Comments

Comments are one of the most important part of any program. In any programming language. They are important because they let us annotate the code and add important information that otherwise would not be available to other people (or ourselves) reading the code.

In JavaScript, we can write a comment on a single line using ```//``` . Everything after ```//``` is not considered as code by the JavaScript interpreter.
Like this:

```
// a comment
true //another comment
```

Another type of comment is a multi-line comment. It starts with ```/*``` and ends with ```*/``` .
Everything in between is not considered as code:

```
/* some kind
of
comment
*/
```


### Semicolons

Every line in a JavaScript program is optionally terminated using semicolons.
I said optionally, because the JavaScript interpreter is smart enough to introduce semicolons for you.
In most cases, you can omit semicolons altogether from your programs.
This fact is very controversial, and you'll always find code that uses semicolons and code that does not.
My personal preference is to always avoid semicolons unless strictly necessary.

### Values

A ```hello``` string is a ***value***. A number like ```12``` is a ***value***.

```hello``` and ```12``` are values. string and number are the ***types*** of those values.

The ***type*** is the kind of value, its category. We have many different types in JavaScript, and we'll talk about them in detail later on. Each type has its own characteristics.

When we need to have a reference to a value, we assign it to a ***variable***. The variable can have a name, and the value is what's stored in a variable, so we can later access that value through the variable name.

### Variables

A variable is a value assigned to an identifier, so you can reference and use it later in the program.

This is because JavaScript is ***loosely typed***, a concept you'll frequently hear about.
A variable must be declared before you can use it.

We have 2 main ways to declare variables. The first is to use ```const``` :

```
const a = 0
```

The second way is use ```let``` :

```
let a = 0
```

What's the difference?
```const``` defines a constant reference to a value. 

This means the reference cannot be changed. You cannot reassign a new value to it.
Using let you can assign a new value to it. 

For example, you cannot do this:

```
const a = 0
a = 1
```

Because you'll get an error: ```TypeError: Assignment to constant variable.`` . 
On the other hand, you can do it using let :

```
let a = 0
a = 1
```

```const``` does not mean "constant" in the way some other languages like C mean. 
In particular, it does not mean the value cannot change - it means it cannot be reassigned. 
If the variable points to an object or an array (we'll see more about objects and arrays later) the content of the object or the array can freely change.

Const variables must be initialized at the declaration time:

```
const a = 0
```

but ```let``` values can be initialized later:

```
let a
a = 0
```

You can declare multiple variables at once in the same statement:

```
const a = 1, b = 2
let c = 1, d = 2
```

But you cannot redeclare the same variable more than one time:

```
let a = 1
let a = 2
```

or you'd get a "duplicate declaration" error.

My advice is to always use ```const``` and only use ```let``` when you know you'll need to reassign a value to that variable. 
Why? Because the less power our code has, the better. If we know a value cannot be reassigned, it's one less source for bugs.

Now that we saw how to work with ```const``` and ```let``` , I want to mention ```var``` .

Until 2015, ```var``` was the only way we could declare a variable in JavaScript.

Today, a modern codebase will most likely just use ```const``` and ```let```.


