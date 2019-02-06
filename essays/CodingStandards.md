---
layout: essay
type: essay
title: Coding Standards
# All dates must be YYYY-MM-DD format!
date: 2019-02-07
labels:
  - Stackoverflow
---
## Introduction
I have always found myself writing code according to some standard to improve my own understanding and readability. When reading others' code I notice following a similar standard to my own improves my ability to understand their code and immediately jump in. Writing code according to a standard improves efficiency, effectiveness, and readability when writing programs.

## Using Coding Standards to Learn a Language


## Coding Standards with Intellij IDEA and ESLint
In this section we will discuss some examples of good and bad questions and how they impacted the result of the inquiry. They showcase in general how a good question can yield far better help than a bad question.


The "good" question, from [stackoverflow](https://stackoverflow.com/questions/236129/how-do-i-iterate-over-the-words-of-a-string), points out the outcome of what the user is trying to do, iterate over the words of a string, rather than the exact method the user is using, such as for loop or while loop. The user is very specific in what current assumptions are in place and what is the desired outcome. The user then displays a full code where anyone can see exactly what the whole program is doing. We see the question below.


> *I'm trying to iterate over the words of a string.*

> *The string can be assumed to be composed of words separated by whitespace.*

> *Note that I'm not interested in C string functions or that kind of character manipulation/access. Also, please give precedence to elegance over efficiency in your answer.*

>  *The best solution I have right now is:*

```c++
#include <iostream>
#include <sstream>
#include <string>

using namespace std;

int main()
{
    string s = "Somewhere down the road";
    istringstream iss(s);

    do
    {
        string subs;
        iss >> subs;
        cout << "Substring: " << subs << endl;
    } while (iss);
}
```
> *Is there a more elegant way to do this?*

We can see on the post that there are 2756 votes at the time of writing this essay and 76 answers. Clearly this post has a helpful answers with this much attention.


We can see with the following "bad" question, from [stackoverflow](https://stackoverflow.com/questions/9564461/jxscrollup-compile), that the user starts out by stating the specific error for the package used and only asks how to compile it. Referencing the question below we see that they failed to identify the root problem they were trying to solve, why they need that package in the first place or what the bigger problem is. This means that there is no room for other alternative suggestions and it is limited to asking only the people that know the exact package they are talking about. The user could have posted this better by elaborating more on the rest of the program they are using or including more source code in addition to using more correct grammar as it appears to be somewhat broken english and cuts out explanations. With a better explanation, they might have been able to provide more information so more potential solutions could be found by other people. We see this question below.

  > *I didn't find a package contains a class JXScrollUp because of sample source code JXScrollupTest.java. I'm using this classpath:*

```java
appframework-1.03.jar:swingx-all-1.6.3.jar:SwingSet3.jar:timingframework-1.0.jar:jgoodies-looks-2.5.0.jar:jgoodies-forms-1.5.0.jar:.).
```
  > *How can I compile it? Many thanks*

  > *Lukas*

## Conclusions
The main things to take away from this essay is that a question needs to be specific in the issue, but provide enough context through describing the room problem so alternative solutions could be found. This in combination with proper grammar and writing to allow people to help you easier will expedite the answering process and make people more likely to provide a solution first of all, and a more quality one.
