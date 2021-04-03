# Introductory HTML and JavaScript

## Structure:
To build a web page we must use a Structure, this will make our web page easy to navigate and helping users to  get the message of the website.

**We use HTML to Structure web pages**

## What is HTML ?
HTML stands for Hyper Text Markup Language, HTML is using to creating web pages.

HTML is consists of a series of elements and it's using them to describes the structure of a Web page.

HTML elements is defined by an opening tag,element attributs, some content, closing tag. 

ex: `<p title="First p">This is a paragraph </p>` 

Tags Tags act like containers & Attributes provide additional information 
about the contents of an element.

***

## Basic HTML page structure:


```
<!DOCTYPE html>

<html>
   <head>
        <title>This is the Title of the Page</title>
   </head>
    <body>
    <h1>This is the Body of the Page</h1>
    <p>Anything within the body of a web page is 
       displayed in the main browser window.</p>
    </body>
</html>

  <head> element contains information about the page.
  <title> The content inside it will be shown in the page's tab.
  <body> The content inside it will be displayed in a browser.
```

### Extra Markup:
```
* <DOCTYPE>: it's a declaration to tell a browser which version of HTML the page is using .
* <!-- -->: this tag is using to add one line or multipul lines comment.
* ID Attribute " it's  used to uniquely identify the element , id is global attribute it's means that every element in HTML can use it. 
* class attribute : it's use to  identify elements.
* <div>: it's container for other html elements.
* ^ <iframe>: is used to embed another page within the current HTML Page.

### Elements Types:
* Block Elements :will always appear to start on a new line in the browser window.
* inline Elements : will always appear to continue on the same line.

### Escape Characters:
* &    &amp;
* "    &quot; 
* ©    &copy;
``` 

## HTML5 Layout:

In the past develpoers used non-semantic elements to built ther web pages.
non-semantic elements  like div tag it's hard to track, then HTML 5 introduces semantic elements that's make our code logical and  more readable .

### semantic elements that we use in html page:
```
* <header>: form it name it's appears at the top of a web page 
* <nav>: it's usually be in the <header> and contains our links
* <main>: it's contain the main contant of our page
* <article>: it's a container for any section of a page 
* <footer>: it's appears at the bottom of a web page
* <hgroup>: it used to group heading elements
* <figure>: it used to contain any content that is referenced from the main flow of an article
```

## Process & Design:

## Process for creating a new website:

### Who is the Site For?
website should be designed for the target audience, and you should know who your target audience is?

this will help you to choose the Appropriate design and contents for your site.

### Why People visit your Website?
you need to consider why people are coming for your website.
Actully vistior coming for two reasons:

1- Key Motivations: 
you need to discover the underlying motivations for them, ex:  If there is a specific goal, isit a personal or professional one. 

2- Specific Goals: 
you need discover to Specific Goals the visitors, Do they want general information, or they want a time 
sensitive information.

### What your visitors are trying to Achieve?

you can create a list of reasons why people would be coming to your site, and you should  looking for key tasks and motivations from their visit. 

### What information your visitors need?

you need to work out what information they need in order to achieve their goals quickly and effectively.

***

## Site Maps:
After you know what is in your site, you need to organize the information into sections or pages.

you need to create a site map, a site map is a diagram of the pages that will be used to structure the site. 

***

## WireFrames:
A wireframe is a simple sketch of the key information that needs to go on each page of a site.


***

## The ABC of Programming

### What is a script and how do I for a create one? 

#### Script Definition:

 is a series of instructions that a computer can follow to achieve a goal, it's similar to a recipe. 

#### How to write a script:

 * Set your goal:you need to define the task you want to achieve.
 * Design the Script:To design a script you split the goal out into a series
 * Code it: Each of the steps needs to be written in a programming language 


### How do computers fit in with the world around them?
Computer creat models of the world using data.

#### Objects & properties:
* Objects: each physical thing in the world can be represented as an object.
* properties: the characteristics of an object, each propertie have it name and value.

#### Event:
An event is the computer's way of sticking up its hand to say, "Hey, this just happened!" 

event can be used to trigger a specific section of the code. 

#### Methods:
methods are actions that can be performed on objects.

*The events, methods, and properties of an object all relate to each other: 
Events can trigger methods, and methods can retrieve or update an 
object's properties.*

#### How a browser sees a web page
1- recive an html page
2- creates a model of the page and store it in the memory
3- shows the page on the screen using a rendering engine
### How do I write a script for a  web page? 
* It is best to keep JavaScript code in its own JavaScript file. 
* The HTML  `<script>` element is used in HTML pages to tell the browser to load the JavaScript file


