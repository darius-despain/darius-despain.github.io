---
layout: essay
type: essay
title: Smart Questions
# All dates must be YYYY-MM-DD format!
date: 2019-01-24
labels:
  - Stackoverflow
---
## Introduction
At some point in every person's career they will run into a problem they cannot solve themselves. To combat this, we ask questions to our peers, supervisors, or public spaces online such as stackoverflow.com. We cannot, however, just give a snippet of the problem and expect someone to help. We must ask questions smartly so we get an effective response in a timely manner. This essay will discuss the topic of asking questions smartly.

## What is a Smart Question?
A smart question, as outlined by Eric Raymond in [his web page on how to ask questions the smart way](http://www.catb.org/esr/faqs/smart-questions.html), is a careful construction of an inquiry to an unknown solution
* The problem is not something already posted to that particular website
* The user has already tried finding the answers in online documentation or other resources
* There is a meaningful subject line
* The question is grammatically correct and formatted properly
*

### Examples
In this section we will discuss some examples of good and bad questions and how they impacted the result of the inquiry. While

#### Good Question
words words.


*I'm trying to iterate over the words of a string.*

*The string can be assumed to be composed of words separated by whitespace.*

*Note that I'm not interested in C string functions or that kind of character manipulation/access. Also, please give precedence to elegance over efficiency in your answer.*

*The best solution I have right now is:*
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
*Is there a more elegant way to do this?*

#### Bad Question



*I didn't find a package contains a class JXScrollUp because of sample source code JXScrollupTest.java. I'm using this classpath:*
```java
appframework-1.03.jar:swingx-all-1.6.3.jar:SwingSet3.jar:timingframework-1.0.jar:jgoodies-looks-2.5.0.jar:jgoodies-forms-1.5.0.jar:.).
```
*How can I compile it? Many thanks*

*Lukas*

## Takeaways
