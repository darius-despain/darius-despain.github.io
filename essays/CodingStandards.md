---
layout: essay
type: essay
title: Coding Standards
# All dates must be YYYY-MM-DD format!
date: 2019-02-07
labels:
  - Intellij IDEA
  - ESLint
---
## Introduction
I have always found myself writing code according to some standard to improve my own understanding and readability. When reading others' code I notice following a similar standard to my own improves my ability to understand their code and immediately jump in. Writing code according to a standard improves efficiency, effectiveness, and readability when writing programs.

## Using Coding Standards to Learn a Language
When I learn a new language, I often conform to the standards of the learning platform I am using to ensure I get the syntax right at first. This shows me exactly how I can write a particular section of code, for example in the following code example I nest my while loop and if statement with tabs such that I can see how the code is organized and I can trace the code better through the flow of the statements.

```js
while(1) {
  if(1) {
    return;
  }
}
```
An experienced coder might not think this is a big deal, but to a new programmer, seeing a rigid structure with defined patterns will squash uncertainty and help them to understand the code easier and faster.

## Coding Standards with Intellij IDEA and ESLint
In this section we will discuss how coding standards with Intellij IDEA and ESLint add to the coding experience.

Intellij IDEA is an IDE that allows for a number of useful features. Included in these is ESLint. ESLint uses a coding standard to check the syntax in a file and notifies the user when a given piece of code does not conform to the standard. While these notifications do not prevent compilation of code, they are used as suggestions so that the user can adjust their code to the standard.

Some users may find this to be a nuisance since it does not hinder operation of the code, but it is a fantastic tool for writing code that conforms to a standard and can even assist the user with making code usable or even fix bugs. For example, when the program defines a variable or function and does not call it, according to the standard we use in ICS 314, ESLint notifies you that the variable or function is never called, which is useful for missing variable reassignments or functions calls when they are supposed to be there. This can be translated into many more of the rules that ESLint catches where it can potentially fix problems in the code before compiling.

## Conclusions
Coding standards can be viewed as an annoyance or inconvenience to some, but there are numerous benefits including better readability, understanding, and ability to learn. In my opinion they should be implemented across all platforms and organizations so that code becomes more uniform and easier to work with.
