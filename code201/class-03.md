# HTML Lists, Control Flow with JS, and the CSS Box Model
## HTML Lists:
* Unordered List: it's start with `<ul>` and each list items start with  '<li>' tag.ul is marked with bullets.
* ordered List: it's start with `<ol>` and each list items start with  '<li>' tag.ol is marked with numbers.
* Definition lists:it's sart with `<dl>`, contain `<dt>` fro the term, and `<dd>` contain the definition.
### All the lists can be nested.

## Boxes:
CSS treats each HTML element as if it lives in its own box. we can customize the box dimensions by suing height and width.

we can limiting the height by using min-height, max-height properties.

we can limiting the width by using min-width, max-width properties.

*Borders, padding, margin they have four values for each other {top right bottom left}

### Overflow:
we use this property to control what happens to content that is too big to fit into the box.

overflow values:
* hidden: hides any extra content that does not fit in the box.
* scroll: add scrollbar to see the rest of the conten.

### Borders:
Every element have a border.to customize an element border we use the following properties:
* border-style : specifies what kind of border to display.like (dotted, dashed, solid, ..etc)
* border-width : specifies the width of the  borders.
* border-color : is used to set the color of the  borders.
###  Margins:
margin properties are used to create space around elements, outside of any defined borders.

we can centering the element by set right & lift margins value to auto.
###  Padding:
Padding is used to create space around an element's content, inside of any defined borders.

### Display:
is used to specifies how an element is displayed. 

Display values:
* block: it's start a new line and take a full with of the page..
* inline: will not start a new line, just take as the width of the element.
* inline-block :will not start a new line but it will act like block element.
* none: it will hide the element without deleting it.

### visibility:
This property is used to hide the element but  leave a space in it place.

### Rounded Corners:
border-radius property, can give any element rounded corners.

## JS:

### Array:
An array is a special variable, used to store multiple values.

we using array when we dealing with list or values are related to each other.

we can creating an array by declaring it name. then assiging it's values in square brackets. ==> var days = ['sun' , 'mon' ,'tue']

### The if Statement:
We use the if statement to specify a block of JavaScript code to be executed if a condition is true.

we use the else if statement to specify a new condition if the first condition is false.
```
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}
```
### Switch:
We use switch statment to perform different actions based on different cases.
```
switch(expression) {
  case x:
    //  block of code
    break;
  case y:
    //  block of code
    break;
  default:
    //  block of code
}
```
### Loop:
loop is used to run a block of code multipule times:
#### for loop syntax:
```
for (initialization; condition; update) {
  // block of code
}
```
### While Loop syntax:
```
while (condition) {
  // code block to be executed
}
```
