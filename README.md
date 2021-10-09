# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a survey of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge.

_You have **three hours** to complete this challenge. Plan your time accordingly._

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results

### Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your team lead as the evaluate your solution.

## Interview Questions

### (please edit this file and write your answer below each question. In addition, you may also review these questions with your mentor)

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Briefly compare and contrast `.forEach` & `.map` (2-3 sentences max)

**Answer**

- .forEach() iterates over every item and executes your function once for each array element. i.e. it doesn't necessarily return anything it just calls the given function for each element.
- .map() does something to every element, returns new array, bascially converts data. The main difference is .map() does "return" values and hence a new array the same "size."

2. Explain the difference between a callback and a higher order function.

**Answer**

- Higher Order Functions (HOF's) take or combine other functions inside themselves. By taking one or more arguments as arugument(s) it can use other functions to accomplish a new task.
- Callback on the other hand is passed into the HOF. It doesn't take other fucntions in as arguments.

3. Can you explain what a closure is and how you used it in the counter function?

**Answer**

- Closure is when a function reaches up (in scope) from the child to parent or outside itself to retrive variable values. In the counter function used variables supplied elsewhere.
 function counterMaker() {
    let count = 0;
    return function counter() {
     return count++;
    }
  }
  here the function counter reaches up to function counterMaker for the count. i.e. where closure occurs.

4. Describe the four principles of the 'this' keyword.

**Answer**

- __Window Binding,__ if you don't define it then you get the whole window back. i.e. you need to give context to the deffinition to "this" otherwise it will return the window, the global object, in node or undefined in 'strict' mode.
- __Implicit Binding__ - 80% of the time binding is implicit. It's when a function is invoked you can look to the left of the dot to determine where "this" is binding.
- __Explicit Binding__ used with .bind() (immediately invokes), .call()(invokes later). The argument is "explicitly" bound to "this"
- __New Binding__ used with the "new" keyword.

5. Why do we need super() in an extended class?

**Answer**

- super is how we call a constructor properties and other methods of the parent class.

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade.

## Instructions

### Task 1: Project Set Up

Follow these steps to set up your project:

1. Fork the repo
2. Clone your forked version of the repo
3. cd into your repo and create a branch with your first and last name
NOTE: Tests will run for the JavaScript portion of this challenge only
4. open the terminal in your vs code and type `npm install`
5. next type `npm run test:watch` in your terminal
6. Complete your work making regular commits, once you have all your tests passing and you are ready to submit your work please see canvas for instructions on how to submit

### Task 2: Project Requirements

Your finished project must include all of the following requirements

#### Task A: Closure

This challenge takes a look at closures as well as scope.
- [ ] Find this challenge in the index.js file. Read the instructions carefully!

#### Task B: Objects and Arrays

Test your knowledge of advanced array methods and callbacks.
- [ ] Find this challenge in the index.js file. Read the instructions carefully!

#### Task C: Prototypes

Create constructors, bind methods, and create cuboids in this prototypes challenge.
- [ ] Find this challenge in the index.js file. Read the instructions carefully!

#### Task D: Classes

Once you have completed the prototypes challenge, it's time to convert all your hard work into classes.
- Find this challenge in the index.js file. Read the instructions carefully!

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

### Task 3: Stretch Goals

There are a few stretch problems found throughout the files, don't work on them until you are finished with MVP requirements! Please remember to comment out your stretch goals before you submit

## Submission format

See Canvas for submission instructions


## Note the difference between parameters and arguments:

  - unction parameters are the names listed in the function's definition. Function arguments are the real values passed to the function. Parameters are initialized to the values of the arguments supplied.

## HOF
  - One of the characteristics of JavaScript that makes it well-suited for functional programming is the fact that it can accept higher-order functions. A higher-order function is a function that can take another function as an argument, or that returns a function as a result.