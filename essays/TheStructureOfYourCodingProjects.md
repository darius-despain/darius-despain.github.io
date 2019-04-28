---
layout: essay
type: essay
title: The Structure of Your Coding Projects
# All dates must be YYYY-MM-DD format!
date: 2019-04-27
labels:
  - Design patterns
---
## Structure of Code
When you create a coding project, it is generally organized in some way. Whether intentional or not, all coding projects have some sort of structure. They can be as simple as relaying all of the stored information directly, or as complicated as an interface to select certain pieces of information and only show the user exactly what they want to see. These structures are called design patterns.

## Examples of Design Patterns
Some examples of types of design patterns one might find are Observer, Singleton, Factory,  and Model-View-Controller (MVC). The Observer design pattern is a completely transparent method where all objects are notified of another's change and then all values are updated automatically. The Singleton design pattern uses a single instance of an object, then continues to use that object for all functions. Factory utilizes it's existing functions to create new objects, so all objects are made based on others and are children of the parent object. MVC is the primary use case in most applications where there is a model layer that manages all the data, but is not displayed to the user, then a view layer that is the platform to display the information to a user, then the controller layer that directs which information from the model to display to the view layer.

## How is this relevant to me?
These patterns may seem like they are useless to the standard coder, but they are good to understand because it may be something you are inadvertently doing with your own code, and understanding these patterns can then help you understand faults that your own code has. In my own code I use the MVC pattern in my final project: Teleskope. This application has a database of companies and students, where they can find each other based on profile information. The MVC pattern means that I have a database that organizes the information, this is the model layer, then a user interface (UI) where the user browses for either companies or students, this is the view layer, and code that sorts the data based on the current user's profile and what matches them, this is the controller layer.

It can be relevant to you to think about this organization so you can understand what role each part of your code has. An example is, by looking at Teleskope, we can see that the view layer is the web interface that displays the companies and students, but the controller layer is the one that directs what information to present to the user, so we have to design code that is responsible for that role by taking data in and processing it to then tell the UI what information it needs to show the user based on the database, the model layer.
