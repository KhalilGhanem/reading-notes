# JS Object Literals; The DOM
## JS Object:
An object is a container for values called properties or methods.
* properties: are an oject variables.
* methods: function that are stored in the object.

We can create an object by using literal notation way.

We can access an object properties and methods by using dot notation. and we can also access an object properties by using square brackets.

ex:
```
let hote l = { 
name: 'Quay', 
rooms: 40, 
booked : 25, 
checkAvailability: function() { 
return this.rooms - this.booked; 
} 
} ; 
```
## The DOM:
is stand for The Document Object Model and it is, basically, a structured representation of HTML documents.
* The DOM allows us to use JavaScript to access and update HTML elements.
* The DOM is a part of the web Application Programming Interfaces(API). that s let humans interact with programs.
* When a browser loads a web page, it creates a DOM tree model, and it is stored in the browsers' memory. 
* DOM tree types of nodes
  * The Document node: is a special object that we have access to in JavaScript.
  * Elements nodes :HTML elements describe the structure of an HTML page.
  * Attribute nodes
  * Text nodes
### Work with the DOM tree
1. Locate the node that represents the element you want to work with. 
  * How We can access the elements 
  * Select an individual element node:
     * `get El ementByld()` Uses the value of an element's id attribute.
     * `querySe1ector()` Uses a CSS selector, and returns the first matching element. 
  * Select multiple elements  (NODELISTS):
    * `getElementsByClassName()` Selects all elements that have a specific value for their class attribute.
    * `getElementsByTagName()` Selects all elements that have the specified tag name .
    * `querySelectorAll()` Uses a CSS selector to select all matching elements. 
  * Traversing between elemets nodes:
    * parentNode Selects the parent of the current element node (which will return just one element). 
    * previousSibl ing / nextSibl ing Selects the previous or next sibling from the DOM tree.
    * firstChild / lastChild Select the first or last child of the current element. 
 
2. Use its text content, child elements, and attributes. 

 ### DOM queries: 
 are the methods that find the element in the DOM tree and it's can returen one element or nodelist.

 we can select element nodes by their id or cl ass attributes, by tag name, or using CSS selector syntax. 

 ### Selecting from nodelist:
 We can Selecting from nodelist in two ways:
 * The item method that return an individual node from the Node list.  ex:` elements.item(O)` this will return the first element.
 * The array syntax: it's the best and the faster way to returns the elements ex:`elements[0]`

 ### using loops to modify the nodelist:
 we can use loops to change the noodlist values. ex:
```
var hotlt ems = document .querySelectorAl l (' l i . hot') ; 
for (var i=O; i<hotl tems.length; i++) {
hotltems[i] .className = 'cool'; }

```
### Access and Change node text:
we can use `textContent` to access and modify nodes text.
* access ex: querySe1ector('.message').textContent;
* modify ex: querySe1ector('.message').textContent='newmessage';

### Add or remove HTML content.
there are two ways to add or remove HTML content.
* The innerHTML
  * adding ex: `.getElementByld('one').innerHTML='new text';`
* The DOM manipulation 










