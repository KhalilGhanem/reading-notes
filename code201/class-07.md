# Object-Oriented Programming, HTML Tables
## HTML Tables
we use `<table>` tag to create tables in HTML.

### Table Structure:
```
* <thead>: contain all the headings of the table.
* <tbody>: contain the body of the table. 
* <tfoot>: contain the table footer.
* <tr>: defined  the table row.
* <td>: defined  the table data.
* <th>: defined  the table header.
```
we can make cells of a table span more than one row 
or column using the rowspan and colspan attributes.

## Functions, Methods, and Objects
### constructor:
A constructor is a function that creates an instance of an object by using new keywords.

creating constructor ex: `let car1 =new oject();` this will make a blank object 
fill an object
```
car1.brand=`Audi`;
ca1.model='A7';
car1.maxspeed=250;
car1.stop(){
    //code;
};
or we can use function tocreate and fill oject
function car1(brand,model,maxspeed){
    this.brand='Audi';
    this.model='A7';
    this.maxspeed=250;
    
    this.stop(){
    //code;
};
}

```
* Array are a special type of object, they holds key/value pairs, but the keys for each value is its index number.
* Arrays and objects can be used to create complex data sets (and both can contain the other). 

### JavaScript built-in objects:
JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts.

built-in objects groups:
* BROWSER OBJECT MODEL: contains objects that represent the current browser window or tab.
  
  ex: window.innerHeight, window.innerWidth, window.pageXOffset
* DOCUMENT OBJECT MODEL: uses objects to create a representation of the current page.

 ex: document.title, document.lastModified, document.URL
* GLOBAL JAVASCRIPT OBJECTS: represent things that the JavaScript language needs to create a model of.

 ex: String objects, number objects, date object







