# Basics of HTML, CSS & JS

## Important HTML tags will help you when you adding text: 
```
*Headings: HTML have six levels of heading from most important heading <H1> to the less important one <H6>.
*Paragraph:  you create paragraph in Html by using <p> Tag.
*Blod: By enclosing words in the tags <b> and </b> we can make characters appear bold.
*Italic: By enclosing words in the tags <i> and </i> we can make characters appear italic.
*superscript: to use superscript in HTML we use <Sup>.
*subscript: to use subscript in HTML we use <sub>.
*Line Breaks: to make a new line in HTML page we use <br> tag.
*Horizontal Line:to make a Horizontal Line In HTML we use <hr> tag, <hr> create a break between elements.
*Strong: <strong> tag is used when you have an important text.
*Emphasis: <em> tag is used if you want to emphasis certain word.
*Blockquote: <blockquote> tag is used for longer quotes that take up an entire paragraph.  
*Quotes: <Q> tag is used for shorter quotes.
*Abbreviations: <abbr> tag is used for Abbreviations.
*Citations: we used <cite> tage when we are referencing a piece of work.
*Definitions: we used <dfn> tag when we explain some new terminology for the first time.
*Address: <address> tag is used  to contain contact details for the author of the page.
*Inserted text: <ins> tag defines a text that has been inserted into a page.
*Deleted text: <del> tag defines a text that has been deleted from a page.
*<s>: the <s> tag specifies text that is no longer correct.
```

***

## Introducing CSS:
CSS allows you to create rules that specify how the content of an element should appear.

CSS rule contains two parts:a selector and a declaration.   `Selector {property:value}`
* The selector:indicate which element the rule applies to.
* Declaration:indicate how the elements referred to in the selector should be styled. Declarations are split into two:
   * property:indicate the aspects of the element you want to change.
   * Value:specify the settings you want to use for the chosen properties.

### Using CSS:
CSS can be added to HTML documents in three ways:

1. Inline: by using the style attribute inside HTML elements.
2. Internal: by using a `<style>` element in the `<head>` section.
3. External: by using a `<link>` element to link to an external CSS file (Best Practice).

### CSS Selectors:
```
*Universal Selector ==> *{} <== Applies to all elements in the document
*Type Selector ==> p,a{} <== Matches element names
*Class Selector ==> p,a{} <== Matches an element whose 
*class attribute ==>.firts{} <== that matches the one specified after the period
*ID Selector ==> #second[] <== that matches the one specified after the hash
*Child Selector ==> li>a {} <== Matches an element that is a direct child of another
*Descendant Selector ==> p a [] <== Matches an element that is a descendent of another specified element 
*Adjacent Sibling Selector ==> h2+a <== Matches an element that is the next sibling of another
*General Sibling Selector ==>h2-a <== Matches an element that is a sibling of another 
```

***

## Basic JavaScript Instructions:
* statements: are programming instructions.
* Comments: is used  to explain what your code does. 
* variables are containers for storing data values.

we must declaring a variables in order to use it. to declare a variable we use var keywords follwoing by variable name ==> var usreAge;

after declaring the variables we can assgin value to it ==> userAge = 25;

### Data types in js:
* String: is set of characters.
* Number: js have one type of numbers
* Booleans: can only have two values: true or false.


### Array:
An array is a special variable, used to store multiple values.

we using array when we dealing with list or values are related to each other.

we can creating an array by declaring it name. then assiging it's values in square brackets. ==> var days = ['sun' , 'mon' ,'tue']

***

## comparison operator:

### evaluating conditions :

we can evaluate a situation by comparing one value in the script to what expect it might be.

*The result will be boolean.*

```
Operators compares two values:
Is Equal to == "see if the values are the same"
Strict Equal to === "check the both data type and the value are the same"
Is not Equal to != "see if the values are not the same"
Strict  Equal === "check the both data type and the value are not the same"
Greater than >
less than <
Greater than or equal to >=
less than or equal to <=
```
### Logical operator

comparison operator usually return true or false. 

logical operators allow you to compare the result of more than one comparison operator.

ex: ((5 < 2) && (2 >=3))

```
&& logical and :this operator test more than one condition
|| logical or : this operator test at least one condition
! logical nor : this operator takes a single boolean value and inverts it.
```

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








 


