---
category: article
tags: javascript
description: Javascript Basics
layout: post
image:
---

I don't work with JavaScript much, but when I do it's handy to have some notes.

1.1 [Introducing JavaScript](#11-intro)
* Learn about the most popular scripting language on the planet. The language that drives millions of interactive web sites, powers fast web servers and can even be used to build desktop applications. In this stage, you'll create your first JavaScript program and learn how to troubleshoot your programming mistakes.

1.2 [Storing and Tracking Information with Variables](#12-variables)
* Learn how to use variables to store information that changes during a program, like the score in a game, or a sales total. You'll also learn about different data types in JavaScript like string, numbers and boolean values.

1.3 [Working With Numbers](#13-numbers)
* Numbers are everywhere in programming. You use them to track a player's score in a game, to calculate the cost of shipping a product, or just to count the number of times a "Like" button was clicked on a page. In this section of the course, you'll learn how to do basic math in JavaScript.

1.4 [Making Decisions with Conditional Statements](#14-conditionals)
* Conditional statements let you control the "flow" of your program. They let you run different code based on conditions in your program.

1.5 [Creating Reusable Code with Functions](#15-functions)
* JavaScript functions are a powerful tool that let you create re-usable chunks of code. They make programming faster, easier and less error-prone. They are also one of the most important concepts in JavaScript programming.

***

### 1.1 Intro
* JavaScript is used to build complex web apps, like GMail, Google Docs, and Google Maps.
* You can use JavaScript on a web server.
* Syntax is like the vocabulary and grammar of the language.  It's a language's commands as well as the instructions for putting them together to create a program.
* JavaScript lets us add interactive components to a site like photo galleries, tabbed panels, or form validation.

#### First JavaScipt Program
* Some common commands and fundamental building block of a program and statement.

```js
alert('Hello World');
document.write("<h1>Welcome to JavaScript Basics</h1>");
alert('thanks for visiting!doc')
```

#### Where Does JavaScipt Go?
* Link a JavaScript file to a web page using the ```<script>``` tag and the src property: 

```javascript
<script src="scripts.js"></script>
```

* Insert JavaScript directly into a web page inside ```<script>``` tags:

```js
<script>
alert("Hello there.");
</script>
```

* Never link to a file and include JavaScript inside the same ```<script>``` tag.
* Place the `<script>` tag in the head or the last line of the body.

#### The JavaScript Console
* Chrome Console Keyboard Shortcuts
  * Mac: Cmd + Option + J

```javascript
alert('hello there');
document.write("Now it works!");
console.log('Program Complete');
```

> When a browser "executes" a JavaScript program, the browser is reading and acting on the JavaScript programming, aka "running" the program.  (Running and Executing a program mean the same thing.)

#### Adding Scripts and Simple JavaScript Commands
* At the beginning of this script on line 9, type the code required to print 'Begin program' to the browser's JavaScript console.
* At the end of this script after the `document.write()`, type the code required to print 'End program' to the browser's JavaScript console.

```html
<!DOCTYPE HTML>
<html>
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  <title>JavaScript Basics</title>
</head>
<body>
<script>
console.log("Begin program");
document.write("Welcome to JavaScript Basics");
console.log("End program");
</script>
</body>
</html>
```

#### Review

* A syntax error is a grammatical mistake like mistyping a JavaScript command or forgetting a closing parentheses or quote mark.
* We use the JavaScript Console to find errors and send hidden messages that show how our program is running.

***

# 1.2 Variables
#### Create a Variable
```js
var message = "Hello!";
alert(message);
message = "Welcome to JavaScript Basics!";
alert(message);
```
> notice the second instance of message, we don't need to define it twice.

#### Naming Variables
* Some words are reserved.
  * [JavaScript Reserved Words](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#Keywords)
  * We can begin a variable name with $ or _.

***

#### Strings and Numbers
* Same rules as Ruby.

***

#### Create a Variable with a String
```js
var player = 'Jasmine';
document.write(player);
```

***

#### Capturing Visitor Input and Writing it to the Page
* The `prompt()` command
  * `prompt()` captures visitor input from a dialog box. You can store that input in a variable like this:
```js
var answer = prompt("What is the color of the moon?");
console.log(answer);
document.write(answer);
alert(answer);
```

***

#### Combining Strings (Concatenation)
```js
var visitor = prompt("What is your name?");
var message = "Hello "
message += visitor
message += ", we are glad you stopped by!";
document.write(message);
```

```js
var firstName = prompt("What is your first name?");
var lastName = prompt("What is your last name?");
var fullName = firstName;
fullName += " ";
fullName += lastName;
console.log(fullName);
alert("Hello " + fullName);
```

***

#### Working with Strings and Finding Help
* use the [Mozilla Developer Network (MDN)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference) to explore the JavaScript language.

* Some String Properties and Methods

  * Property `.length` returns the number of characters inside a string
```js
var str = '9 letters';
alert( str.length ); 
// opens an alert dialog with the number 9
```
  * Method `.toUpperCase()` returns a copy of a string with all uppercase letters
```js
var str = 'upper';
alert( str.toUpperCase() ); 
// opens an alert dialog with the string 'UPPER'
```
  * Method `.toLowerCase()` returns a copy of a string with all lowercase letters
```js
var str = 'LOWER';
alert( str.toLowerCase() ); 
// opens an alert dialog with the string 'lower'
```
```js
var passphrase = "Open Sesame";
console.log(passphrase.length);
console.log(passphrase.toLowerCase());
console.log(passphrase.toUpperCase());
```
```js
var stringToShout = prompt("What shall I shout?");
var shout = stringToShout.toUpperCase();
shout += "!!!";
alert(shout);
```

***

#### Review
```js
var adjective = prompt("type an adjective");
var verb = prompt("type a verb");
var noun = prompt("type a noun");
alert("you're done");
document.write("<h2>"+ adjective + " " + noun + " " + verb +"</h2>");
```

***

# 1.3 Numbers
#### Storing Numbers in Variables
```javascript
var age = 40; // Integer
var price = 1.99; // Float
var miles = "200"; // String
```

#### Doing Math
> console: NaN means "not a number".

#### Numbers and Strings
```javascript
var str = '49 steps';
var num = parseInt(str);
// num now holds the number 49

var str = '102.99%';
var num = parseFloat(str);
// num now holds the number 102.99
```
#### Challenge
_index.html_
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <link rel="stylesheet" href="css/main.css">
  <title>The Story Maker</title>
 </head>
<body>
  <div class="container">
  <h1>The Story Maker</h1>
  <script src="story.js"></script>
  </div>
</body>
</html>
```
_story.js_
```javascript
var questions = 3;
var questionsLeft = ' [' + questions + ' questions left]';
var adjective = prompt('Please type an adjective' + questionsLeft);
questions -= 1;
questionsLeft = ' [' + questions + ' questions left]'
var verb = prompt('Please type a verb' + questionsLeft);
questions -= 1;
questionsLeft = ' [' + questions + ' questions left]'
var noun = prompt('Please type a noun' + questionsLeft);
alert('All done. Ready for the message?');
var sentence = "<h2>There once was a " + adjective;
sentence += ' programmer who wanted to use JavaScript to ' + verb;
sentence += ' the ' + noun + '.</h2>';
document.write(sentence);
```
#### The Math Object
[Mozilla Developer Network page on the Math object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)
#### Using Math Methods
```javascipt
var temperature = 37.5;
alert(Math.round(temperature));
alert(Math.floor(temperature));
```
#### Create a Random Number
_index.html_
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <link rel="stylesheet" href="css/main.css">
  <title>Random Number!</title>
 </head>
<body>
  <div class="container">
  <h1>Random Number</h1>
  <script src="app.js"></script>
  </div>
</body>
</html>
```
_app.js_
```javascript
var dieRoll = Math.floor(Math.random() * 6) + 1;
document.write(dieRoll);
```
or...
_index.html_
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <link rel="stylesheet" href="css/main.css">
  <title>Random Number!</title>
 </head>
<body>
  <div class="container">
    <h1>Random Number</h1>
    <script src="random.js"></script>
  </div>
</body>
</html>
```
_random.js_
```javascript
var input1 = prompt("Pleast type your first number");
var number1 = parseInt(input1);
var input2 = prompt("Please your second number");
var number2 = parseInt(input2);
var randomNumber = Math.floor(Math.random() * (number1 - number2 + 1)) + number2;
var message = "<p>" + randomNumber + " is a number between " + number2 +  " and " + number1 + ".</p>";
document.write(message);
```

***

# 1.4 Conditionals
How JavaScript programs react intelligently based on the input provided by users or conditions within the program itself.

_index.html_
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <link rel="stylesheet" href="css/main.css">
  <title>A programming quiz</title>
 </head>
<body>
  <div class="container">
  <h1>A programming quiz</h1>
   <script src="quiz.js"></script> 
  </div>
</body>
</html>
```
_quiz.js_
```javascript
var answer = prompt("What programming language is best?");
if ( answer.toUpperCase() === "JAVASCRIPT") {
  document.write("<p>Correct!</p>")
} else {
  document.write("<p>Wrong, JavaScript is the best!.</p>")
}
```
#### Comparison Operators
* (3>2) is true
* ("apple" < "bear") is true
* ("3" == 3) is true
* ("3" === 3) is false, 'strict equality' operator.
* (100 <= 100) is true
* (100 !== 100) is false, strict 'not equals' operator

#### Random Number Guessing Game
_index.html_
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <link rel="stylesheet" href="css/main.css">
  <title>Random Number Guessing Game</title>
 </head>
<body>
  <div class="container">
  <h1>Random Number Guessing Game</h1>
   <script src="script.js"></script> 
  </div>
</body>
</html>
```
_script.js_
```javascript
var randomNumber = Math.floor(Math.random() * 6 ) + 1;
var guess = prompt("I am thinking of a number between 1 and 6, what is it?");
if (parseInt(guess) === randomNumber ) {
  document.write("<p>You guessed the number!</p>");
} else {
  document.write("<p>Sorry, The number was " + randomNumber + "</p>");
}
```
#### Boolean Values
same _index.html_

_script.js_
```javascript
var correctGuess = false;
var randomNumber = Math.floor(Math.random() * 6 ) + 1;
var guess = prompt('I am thinking of a number between 1 and 6. What is it?');
if (parseInt(guess) === randomNumber ) {
  correctGuess = true;
}
if (correctGuess ) {
  document.write('<p>You guessed the number!</p>');
} else {
  document.write('<p>Sorry. the number was ' + randomNumber + '</p>');
}
```
#### Improving the Random Number Guessing Game with if/else
same _index.html_

_script.js_
```javascript
var correctGuess = false;
var randomNumber = Math.floor(Math.random() * 6 ) + 1;
var guess = prompt('I am thinking of a number between 1 and 6. What is it?');
if (parseInt(guess) === randomNumber ) {
  correctGuess = true;
} else if (parseInt(guess) < randomNumber) {
  var guessMore = prompt('Try again. The number I am thinking of is more than ' + guess);
  if (parseInt(guessMore) === randomNumber) {
    correctGuess = true;
  }
} else if (parseInt(guess) > randomNumber) {
  var guessMore = prompt('Try again. The number I am thinking of is less than ' + guess);
  if (parseInt(guessMore) === randomNumber) {
    correctGuess === true;
  }
}
if ( correctGuess ) {
    document.write('<p>You guessed the number!</p>');
} else {
    document.write('<p>Sorry. The number was ' + randomNumber + '</p>'); 
}
```
#### Documenting Code with Comments
same _index.html_

_script.js_
```javascript
/*
The Random Number Guessing Game
Generates a number between 1 and 6
and gives a player two attempts to
guess the number.
*/

// assume the player didn't guess correctly
var correctGuess = false;

// generate a random number from 1 to 6
var randomNumber = Math.floor(Math.random() * 6 ) + 1;

var guess = prompt('I am thinking of a number between 1 and 6. What is it?');

/* test to see if player
1. is correct
2. guessed too high
3. guessed too low
*/
if (parseInt(guess) === randomNumber ) {
  correctGuess = true;
} else if (parseInt(guess) < randomNumber) {
  var guessMore = prompt('Try again. The number I am thinking of is more than ' + guess);
  if (parseInt(guessMore) === randomNumber) {
    correctGuess = true;
  }
} else if (parseInt(guess) > randomNumber) {
  var guessMore = prompt('Try again. The number I am thinking of is less than ' + guess);
  if (parseInt(guessMore) === randomNumber) {
    correctGuess === true;
  }
}

// test if player is correct and output response
if ( correctGuess ) {
    document.write('<p>You guessed the number!</p>');
} else {
    document.write('<p>Sorry. The number was ' + randomNumber + '</p>'); 
}
```
#### Combining Multiple Tests Into a Single Condition
```javascript
/*
Challenge Instructions

1. Ask at least five questions

2. Keep track of the number of questions the user answered correctly

3. Provide a final message after the quiz letting the user know the number of questions he or she got right.

4. Rank the player. If the player answered all five correctly, give that player the gold crown: 3-4 is a silver crown; 1-2 correct answers is a bronze crown and 0 correct is no crown at all.
*/

// quiz begins, no answers correct
var correct = 0;

var q1 = prompt("Who won the 2012 Eufa Champions League?");
if ( q1.toUpperCase() === "CHELSEA" ) {
  alert( "Correct!");
  correct += 1;
} else {
  alert( "Wrong!");
}
alert(correct + " of 5 correct thus far");

var q2 = prompt("Who won the 1986 Super Bowl?");
if ( q2.toUpperCase() === "CHICAGO" || q2.toUpperCase() === "BEARS" || q2.toUpperCase() === "CHICAGO BEARS" ) {
  alert( "Correct!");
  correct += 1;
} else {
  alert( "Wrong!");
}
alert(correct + " of 5 correct thus far");

var q3 = prompt("Who won the 1995 College Football National Championship?");
if ( q3.toUpperCase() === "NEBRASKA" ) {
  alert( "Correct!");
  correct += 1;
} else {
  alert( "Wrong!");
}
alert(correct + " of 5 correct thus far");

var q4 = prompt("Who won the 2016 NBA Finals?");
if ( q4.toUpperCase() === "CLEVELAND" ) {
  alert( "Correct!");
  correct += 1;
} else {
  alert( "Wrong!");
}
alert(correct + " of 5 correct thus far");

var q5 = prompt("Who won the 2016 World Series?");
if ( q5.toUpperCase() === "CHICAGO CUBS" || q5.toUpperCase() === "CUBS" ) {
  alert( "Correct!");
  correct += 1;
} else {
  alert( "Wrong!");
}
alert(correct + " of 5 correct!");

// Final message and rank.
if ( correct === 5) {
  document.write("<p>You won the gold crown!</p>");
} else if ( correct >= 3) {
  document.write("<p>You won the silver crown!</p>");
} else if ( correct >= 1) {
  document.write("<p>You won the bronze crown!</p>");
} else {
  document.write("<p>You win nothing!</p>");
}
```
***

# 1.5 Functions
Declaring a function
```javascript
function myFunction() {
  // do a bunch of stuff here
}
```
Calling a function
```javascript
myFunction();
```
A function expression (won't use in this wiki, FYI.)
```javascript
var myFunction =  function () {
  // do stuff here
};
```
[Function Information from Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/function)
#### Creating a Function
```javascript
// Declare the function.
function alertRandom() {
  var randomNumber = Math.floor( Math.random() * 6 ) + 1;
  alert(randomNumber);
}

// Call the function.
alertRandom();
```
#### Getting Information From a Function
```javascript
function getRandomNumber() {
  var randomNumber = Math.floor( Math.random() * 6 ) + 1;
  return randomNumber;
}
alert( getRandomNumber() );
console.log ( getRandomNumber() );
var dieRoll = getRandomNumber();
```
#### Giving Information to Functions
```javascript
function getRandomNumber( upper ) {
  var randomNumber = Math.floor( Math.random() * upper ) + 1; 
  return randomNumber;
}
/*
console.log( getRandomNumber(6) );
console.log( getRandomNumber(100) );
console.log( getRandomNumber(10000) );
console.log( getRandomNumber(2) );
*/
function getArea( length, width, unit ) {
  var area = length * width;
  return area + " " + unit;
}
console.log(getArea( 10, 20, "sq ft" ));
```
* In JavaScript, "scope" refers to where in a program a variable can be accessed.
* A JavaScript argument is a value you can pass to the function when you call the function.
#### Variable Scope
* How JavaScript protects variables from writing over each other.
* [Everything you wanted to know about JavaScript scope](https://toddmotto.com/everything-you-wanted-to-know-about-javascript-scope/)
```javascript
function greeting(){
  // function scope for var person
  var person = "Lyla";
  return person;
}
// global scope for var person
var person = "Rocco";
console.log(greeting()); // Lyla
console.log(person); // Rocco
```
* Always use the 'var' keyword when creating a variable inside a function.
* If you don't, your function reaches out to the global variable and might overwrite a variable of the same name.
```javascript
function greeting(){
  // function scope for person
  person = "Lyla";
  return person;
}
// global scope for var person, function overrides var person
var person = "Rocco";
console.log(greeting()); // Lyla
console.log(person); // Lyla
```
#### Random Number Challenge
```javascript
function getRandomNumber( lower, upper ){
  if ( isNaN(lower) || isNaN(upper) ) {
    throw new Error("both arguments must be numbers!");
  } else {
    return Math.floor(Math.random() * ( upper - lower + 1)) + lower;   
  }
}

console.log( getRandomNumber( 'nine', 24 ) ); // Uncaught Error: both arguments must be numbers!(…)
console.log( getRandomNumber( 1, 100 ) );
console.log( getRandomNumber( 200, 'five hundred' ) );
console.log( getRandomNumber( 1000, 20000 ) );
console.log( getRandomNumber( 50, 100 ) );
```