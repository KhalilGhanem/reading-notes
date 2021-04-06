# HTML Links, JS Functions, and Intro to CSS Layout

## HTML lINKS:
Link is used to move from page to another. 
* we can create an HTML link by using `<a>` tags.
* href attribute,is indicates the link's destination.
* we can use target attribute to specifies where the link wil open. target values `_self, _blank,_parent, _top`.
* URLs:
  * Absolute URL: is used for an external link.
  * Relative URL: is used for  a local link.
* We can link a part of the same page by using element id in a tag ex`<a href=#firstp>First paragraph</a>`.
* We can Link to an Email Address by using mailto attribute ex`<a href="mailto:khalil_ghanem7@yahoo.com">Send email</a>`;

***

## CSS Layout:
### The position Property
it's specifies the type of positioning method used for an element.

position values:
* static: the element that use it, will not affected by the top, bottom, left, and right properties.
* relative: the element that use it, will  be adjusted away from its normal position if we use top, bottom, left, and right properties.
* absolute: the element that use it, will  positioned relative to the nearest parent element , or il will use the body.
* fixed: the element that use it, will be in the same place even if we scroll 

***
## JS Functions
A JavaScript function is a block of code designed to perform a specific task.

Function Syntax:
```
function name(parameter1,parameter1){
    blokc of code;
}
```
The function will excute when we call it in the code.

we use return to get the value out of function, but when the js reaches a return statement, the function will stop executing.

we can create a function in two ways:
* FUNCTION DECLARATION 
```
function area (width, height) {
return width * height; 
}; 
```
* FUNCTION EXPRESSION 
```
var ar ea = f unction(width, height) { 
return width * height; 
};
```

## 6 Reasons for Pair Programming :
### pair programming:
is one of the programming styles and it's involves two roles: the Driver and the Navigator.
* The Driver is the programmer who is typing the code .
* The Navigator is the one who guide the Driver.
### Why pair program?
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness