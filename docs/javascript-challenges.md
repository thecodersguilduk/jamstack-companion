---
title: JavaScript Challenges
date: 2021-02-06
slug: javascript-challenges

---
## Variables and Operators

### The Age Calculator

Forgot how old someone is? Calculate it!

1. Store the current year in a variable.
2. Store their birth year in a variable.
3. Calculate their 2 possible ages based on the stored values.
4. Output them to the screen like so: “They are either NN or NN”, substituting the values.

### The Fortune Teller

Why pay a fortune teller when you can just program your fortune yourself?

1. Store the following into variables:
   * number of children
   * partner’s name
   * geographic location
   * job title
2. Output your fortune to the screen like so: “You will be a X in Y, and married to Z with N kids.”

### Using Math functions

JavaScript has a built-in tool that can generate a random number between 0 and 1. This tool is called a _method_. We’ll talk about methods more later in the class. For now, know if you type `Math.random()`, you’ll get a random number between 0 and 1.

Using this tool, update your fahrenheit to celsius temperature conversion program to do the following:

1. Instead of inputing a value for the Fahrenheit temperature, use Math.random() to generate a random temperature between 0 and 100
2. Have to program output: “It is NN°F today. That’s NN°C.”

### The Temperature Converter

Let’s make a program to convert celsius temperatures to fahrenheit and vice versa, so we can complain about the weather with our friends overseas.

**Reminder:** To convert celsius to fahrenheit, multiply by 9, then divide by 5, then add 32. To convert fahrenheit to celsius, deduct 32, then multiply by 5, then divide by 9.

**Unicode Characters:** To print the degrees symbol in JavaScript, we need to use the write \\u00B0 to represent the unicode character for the degrees symbol.

1. Store a celsius temperature into a variable.
2. Convert it to fahrenheit and output “NN°C is NN°F”.
3. Now store a fahrenheit temperature into a variable.
4. Convert it to celsius and output “NN°F is NN°C.”

## Functions and Control Flow

### What number is bigger?

Write a function that compares two numbers and returns the larger one. Be sure to try it out with some different numbers. Bonus: add error messages if the numbers are equal or cannot be compared.

Don’t forget to test it!

### The Calculator

1. Write a function called `squareNumber` that will take one argument (a number), square that number, and return the result. It should also log a string like “The result of squaring the number 3 is 9.”
2. Write a function called `halfNumber` that will take one argument (a number), divide it by 2, and return the result. It should also log a string like “Half of 5 is 2.5.”.
3. Write a function called `percentOf` that will take two numbers, figure out what percent the first number represents of the second number, and return the result. It should also log a string like “2 is 50% of 4.”
4. Write a function called `areaOfCircle` that will take one argument (the radius), calculate the area based on that, and return the result. It should also log a string like “The area for a circle with radius 2 is 12.566370614359172.”
   * **Bonus:** Round the result so there are only two digits after the decimal.
5. Write a function that will take one argument (a number) and perform the following operations, using the functions you wrote earlier:
   1. Take half of the number and store the result.
   2. Square the result of #1 and store that result.
   3. Calculate the area of a circle with the result of #2 as the radius.
   4. Calculate what percentage that area is of the squared result (#3).

### FixStart

Create a function called `fixStart`. It should take a single argument, a string, and return a version where all occurrences of its first character have been replaced with ‘*****’, except for the first character itself. You can assume that the string is at least one character long. For example:

    fixStart('babble'): 'ba**le'
    fixStart('turtle'): 'tur*le'
    

### The Fortune Teller: With Functions!

Let’s turn one of the Class 1 Exercises into a function.

1. Write a function named `tellFortune` that:
   * takes 4 arguments: number of children, partner’s name, geographic location, job title.
   * outputs your fortune to the screen like so: “You will be a X in Y, and married to Z with N kids.”
2. Call that function 3 times with 3 different values for the arguments.

### Pluralise

Write a function `pluralise` that takes in two arguments, a number and a word, and returns the plural. For example:

    pluralise(5, 'cat'): '5 cats'
    pluralise(7, 'turtle'): '7 turtles'
    

Bonus: Make it handle a few collective nouns like “sheep” and “geese”.

### Challenge Question: String Manipulation

If you feel comfortable with the other exercises, it’s time to expand your knowledge! These puzzles involve manipulating strings; to try them out, you’ll need to use some of the [built-in JavaScript methods for strings](http://www.w3schools.com/jsref/jsref_obj_string.asp). Methods are pre-written functions that are built into the language.

These questions are not as straightforward as the others. They challenge you to really think like a programmer. Really try to solve them before you peek at the answer.

### MixUp

Create a function called `mixUp`. It should take in two strings, and return the concatenation of the two strings (separated by a space) slicing out and swapping the first 2 characters of each. You can assume that the strings are at least 2 characters long. For example:

    mixUp('mix', 'pod'): 'pox mid'
    mixUp('dog', 'dinner'): 'dig donner'
    

## Loops, Arrays and Objects

### Even/Odd Counter

Write a for loop that will iterate from 0 to 20. For each iteration, it will check if the current number is even or odd, and report that to the screen (e.g. “2 is even”)

### The Reading List

Keep track of which books you read and which books you want to read!

1. Create an array of objects, where each object describes a book and has properties for the title (a string), author (a string), and alreadyRead (a boolean indicating if you read it yet).
2. Iterate through the array of books. For each book, log the book title and book author like so: “The Hobbit by J.R.R. Tolkien”.
3. Now use an if/else statement to change the output depending on whether you read it yet or not. If you read it, log a string like ‘You already read “The Hobbit” by J.R.R. Tolkien’, and if not, log a string like ‘You still need to read “The Lord of the Rings” by J.R.R. Tolkien.’

### Recipe

Create an object to hold information on your favourite recipe. It should have properties for:

1. `recipeTitle` (a string)
2. `servings` (a number)
3. `ingredients` (an array of strings)
4. `directions` (a string)

Try displaying some information about your recipe.

_Bonus:_ Create a loop to list all the ingredients.

#### Function

Add a function called `letsCook` that says “I’m hungry! Let’s cook…” with the name of your recipe title.

Call your new method.

### Times Tables

Write a program to output the times tables from 1 through to 12. Use a loop within a loop.

### For Loop

[`for`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for) loops - declare a counter in the statement

    // will count 1 to 10
    for (var i = 1; i <= 10; i++) {
      console.log(i);
    }
    

### Loops and Logic

    // Count from 1 to 100
    
    for (var i = 1; i <= 100; i++) {
      if (i % 3 === 0) {
        // Says 'Fizz' after multiples of three
        console.log(' Fizz');
      } else if (i % 5 === 0) {
        // Says 'Buzz' after multiples of five
        console.log(' Buzz');
      } else {
        console.log(i);
      }
    }
    

### Break

To exit a loop, use the [`break`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/break) statement.

    // Count from 100 to 200
    for (var i = 100; i <= 200; i++) {
      console.log('Testing ' + i);
    
      //Stop at the first multiple of 7
      if (i % 7 == 0) {
        console.log('Found it! ' + i);
        break;
      }
    }
    

## Top Choice

Create an array to hold your top choices (colors, presidents, whatever). For each choice, log to the screen a string like: “My #1 choice is blue.”

**Bonus:** Change it to log “My 1st choice, “My 2nd choice”, “My 3rd choice”, picking the right suffix for the number based on what it is. [The method slice](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/slice) might be helpful here.

## The DOM

About Me

Start with this HTML

    <!DOCTYPE html>
    <html>
     <head>
      <meta charset="utf-8"/>
      <title>About Me</title>
    </head>
    <body>
      <h1>About Me</h1>
    
      <ul>
        <li>Nickname:
          <span id="nickname"></span>
        </li>
        <li>Favorites:
          <span id="favorites"></span>
        </li>
        <li>Hometown:
          <span id="hometown"></span>
        </li>
       </ul>
    
     </body>
    </html>
    

1. (In JavaScript) Change the body tag’s style so it has a font-family of “Arial, sans-serif”.
2. (In JavaScript) Replace the content of each of the spans (nickname, favorites, hometown) with your own information.
3. Iterate through each li and add a class of “listitem”. Add a style tag that sets a rule for “listitem” to make the color red.
4. Create a new img element and set its src attribute to a picture of you. Append that element to the body.

### Logo Hijack

1. Open up www.google.com in Chrome or Firefox, and open up the console.
2. Find the Google logo and store it in a variable.
3. Modify the source of the logo IMG so that it’s a Yahoo logo instead. ([http://www.logostage.com/logos/yahoo.GIF](http://www.logostage.com/logos/yahoo.GIF "http://www.logostage.com/logos/yahoo.GIF"))

### The Reading List Part II

1. Create a webpage with an `h1` of “My Book List”.
2. Copy the array of books from the previous exercise.
3. Iterate through the array of books. For each book, create a `p` element with the book title and author and append it to the page.
4. **Bonus:** Use a `ul` and `li` to display the books.
5. **Bonus:** add a property to each book with the URL of the book cover, and add an `img` element for each book on the page.
6. **Bonus:** Change the style of the book depending on whether you have read it or not.

### Challenge Question: The Counter

Write a function that takes a certain type of tag and counts the number of elements with that tag. The function should return “There a X tags of type y on the page. For example:

    countTags('p'): 'There are 3 tags of type p on the page'
    

* [](https://bootcamp.wdan.uk/feed.xml "RSS")