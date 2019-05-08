---
layout: essay
type: essay
title: Going Beyond HTML and CSS
# All dates must be YYYY-MM-DD format!
date: 2019-02-21
labels:
  - HTML
  - CSS
  - Semantic UI
---

<!-- UI Frameworks are not simple. In fact, they can be almost as complicated to learn as a new programming language. Given that, why bother to use something like Semantic UI? What does one get in return for the investment of time and frustration? Why not just use raw HTML and CSS? Are the software engineering benefits of UI frameworks?

          For this assignment, create an engaging and informative essay about UI Frameworks. You might want to discuss some of the issues raised above, as well as your own personal experience with Semantic UI. Or perhaps you’ve also used another framework such as Twitter Bootstrap. In that case, it might be interesting to read your perspective on a comparison of the two.

          Feel free to go in another direction entirely, as long as you are discussing UI Frameworks, and as long as the result is interesting, informative, and insightful. Write for the world!

-->

## Introduction
Sometimes code can get complicated enough to where it is not efficient to write all your own material. This can be seen in many development environments such as prewritten functions and classes for object oriented languages or UI frameworks in web development, enabling users to save time with complicated layouts rather than writing with raw HTML and CSS. This essay will discuss the benefits and drawbacks of using UI frameworks in web development.

## Standard HTML and CSS
HTML is the language web development is based around to organize content and enable links or other functions. It is somewhat tedious of a language as each element must be called directly. An example of HTML and CSS and what it displays can be seen below.
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>A history of surfing</title>
  <link rel="stylesheet" type="text/css" href="style.css" media="screen" />
  <link rel="stylesheet" href="//fonts.googleapis.com/css?family=Hanalei+Fill|Fahkwang" />

</head>
<body>
<h1>A history of surfing</h1>
<p>
  Surfing is a surface water sport in which the wave rider, referred to as a surfer, rides on the forward or deep face of a moving wave, which usually carries the surfer towards the shore. Waves suitable for surfing are primarily found in the ocean, but can also be found in lakes or rivers in the form of a standing wave or tidal bore. However, surfers can also utilize artificial waves such as those from boat wakes and the waves created in artificial wave pools.
</p>
<p>
  Synchronized surfing, Manly Beach, New South Wales, Australia, 1938–46
  The term surfing refers to the act of riding a wave, regardless of whether the wave is ridden with a board or without a board, and regardless of the stance used. The native peoples of the Pacific, for instance, surfed waves on alaia, paipo, and other such craft, and did so on their belly and knees. The modern-day definition of surfing, however, most often refers to a surfer riding a wave standing up on a surfboard; this is also referred to as stand-up surfing.
</p>
<h2>Profiles</h2>
<img src="https://www.surfholidays.com/assets/images/blog/2015-04-28-Surfing-Animals-Seal.jpg" align="middle">
<img src="https://i.ytimg.com/vi/ElFAEazE3Y8/maxresdefault.jpg" align="middle">
<img src="https://i.pinimg.com/originals/1f/e2/47/1fe247334a3d8b3ac34e0217ef198f8b.jpg" align="middle">
<img src="https://www.surfdogricochet.com/uploads/2/1/8/0/21802576/surf-dog-san-diego_1_orig.jpg" align="middle">
</body>
</html>
```
```css
body {
  color: white;
  background-image: url("https://wallpapercave.com/wp/ctumxYy.jpg");
  font-family: "Fahkwang", sans-serif;
}
h1 {
  text-align: center;
  font-family: "Hanalei Fill", sans-serif;
  font-size: 45pt;
}
h2 {
  text-align: center;
  font-family: "Hanalei Fill", sans-serif;
  font-size: 30pt;
}
img {
  width: 300px;
  height: 250px;
}

```
<img class="ui image" src="{{ site.baseurl }}/images/historyofsurfing.png">

As you can see, it takes quite a bit of code, just to put a few images and some text on a screen. This page does not even have fancy layouts or extra menus at the top or bottom and we had to control the sizes of the images manually and the alignment of the text with CSS.  

## Benefits of UI Frameworks
Now that we have seen plain HTML and CSS, let us take a look at some HTML and CSS using semantic UI, a UI framework that enables formatting without the need for tons of CSS accompanying the HTML.
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Starbucks - The Best Coffee and Espresso Drinks</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/semantic-ui/2.4.1/semantic.min.css">
  <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/semantic-ui/2.4.1/semantic.min.js"></script>
  <link rel="stylesheet" href="style.css">
</head>
<body>
<div class="top_green_bar"></div>

<div class="ui container">
  <img class="left floated image" src="https://www.starbucks.com/static/images/global/logo.svg" style="padding: 50px 0px 0px 0px;">
  <div class="ui borderless topmenu menu">
    <a class="right item">COFFEE</a>
    <a class="item">TEA</a>
    <a class="item">MENU</a>
    <a class="item">COFFEEHOUSE</a>
    <a class="item">SOCIAL IMPACT</a>
    <a class="item">STARBUCKS REWARDS</a>
    <a class="item">STORIES</a>
    <a class="item">GIFT CARDS</a>
  </div>
</div>
<div class="main-banner">
  <div class="ui two column middle aligned grid container">
    <div class="column">
      <h1>Love your drink</h1>
      <h4>Choose your espresso, smooth or bold. Discover a drink that's made for you. </h4>
      <button class="ui inverted button">FIND YOUR ESPRESSO</button>
    </div>
  </div>
</div>
```
```css
.ui.borderless.topmenu.menu{
  background-color: white;
  box-shadow: none;
  border: none;
  height: 10px;
  font-size: 13pt;
  color: #1e1e1e;
}
.top_green_bar{
  background-color: #006341;
  min-height: 10px;
}
.main-banner{
  background-image: url("http://globalassets.starbucks.com/assets/01e1dd5076914ee48f267e376491059c.jpg");
  background-position: center;
  min-height: 400px;
  color: white;
  padding-top: 125px;
}
.black-banner{
  background-color: black;
  min-height: 150px;
  color: white;
  padding-top: 5%;
  padding-bottom: 5%;
}
.white-banner{
  background-color: white;
  min-height: 150px;
  color: black;
  padding-top: 5%;
  padding-bottom: 5%;
}
.green-banner{
  background-color: #1b3c35;
  min-height: 150px;
  color: white;
  padding-top: 5%;
  padding-bottom: 5%;
}
.footer{
  background-color: white;
  color: black;
}
```

<img class="ui image" src="{{ site.baseurl }}/images/starbucks.png">

We can see this code is longer yes, but it enables the buttons and menu bars you see in the screenshot as well as multiple layers of items with a more aesthetically pleasing layout. This same layout, if not using semantic UI, would take up an additional page of CSS to format the margins, pattern, alignment, and other functional pieces. In this sense semantic UI allows this website to be more powerful and have more features integrated without too much extra time spent developing the webpage.

This use of premade classes is similar to using other development environments in other languages that might have prewritten pieces of code to use, an example of this is functions in c++ that we can call or in a GUI where blocks of code are prewritten and one just has to call them and assign variables to write a powerful piece of code.

In my experience so far the benefits have been the functionality bump in my sites without having to write extra code, saving me time on homework assignments and able to focus more on implementing the layout I want rather than the syntax to work out the exact spacing. It has also been useful as semantic UI has icons and buttons which I would not normally have access to and would take lots of research to find the image to upload and size it or write a piece of code to design a button, where it takes 1 line of semantic UI to fix this.
## Drawbacks of UI Frameworks
UI frameworks, such as semantic UI, also have drawbacks to their added functionality. Some problems come just from the fact of complicating the code with fancy formatting options where a simple HTML and CSS site with little formatting might be sufficient in certain use cases. This is evident in the two example code pieces shown in this essay where the code using semantic UI was much longer than the vanilla HTML.

Other problems include extra bugs with the added functionality. As you call different classes, some combinations of classes might not behave exactly as one would expect, where some existing class might be taking priority over another and overwriting your formatting written for your website. This can be quite frustrating and cause many hours of troubleshooting or needless code to overwrite something that should have worked in the first place.
## Conclusions
Overall, UI frameworks exist to make web development more functional and aesthetically pleasing while saving time for developers. There are benefits and drawbacks, but this is something each developer should weigh out. For example, if a site is needed simply to post a few links and text lines for a small amount of users, it might be more advantageous to not use a UI framework as it would result in less lines of code and therefore time saves. On the other hand, a developer building a website for a company should definitely use a UI framework to attract more people to the site and make it easier to use, all while allowing expandability of features for the site.
