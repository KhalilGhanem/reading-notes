# React and Forms

1. What is a ‘Controlled Component’?

   The form data that is handled and controlled by React. 

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

    We should uspdate the state as soon as the user enter them, because we may need the state value in alert or other stuff.

3. How do we target what the user is entering if we have an event handler on an input field?
    
    We can use event parameter to get access to Value attribute. 

## The Conditional (Ternary) Operator Explained
1. Why would we use a ternary operator?

    it makes the code easier to read
    
2. Rewrite the following statement using a ternary statement:
```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
======================>
x==y ?console.log(true):console.log(false);
 
```