# Maps, primitives, File I/O

## Primitives versus Objects
Java has a two type system consisting of :

* Primitives: int, boolean.
* Reference type: nteger, Boolean. 

Java performs a conversion between the primitive and reference types 
```
Integer j = 1;          // autoboxing
int i = new Integer(1); // unboxing
```
The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.

### Size on memory :

1- primitives

  * boolean – 1 bit
  * byte – 8 bits
  * short, char – 16 bits
  * int, float – 32 bits
  * long, double – 64 bits

These values can vary depending on the Virtual Machine implementation and they are lives in the stack and hence.

2- Reference

  * Boolean – 128 bits
  * Byte – 128 bits
  * Short, Character – 128 bits
  * Integer, Float – 128 bits
  * Long, Double – 192 bits

 The reference types are objects, they live on the heap.

 Summary:  The primitive types are much faster and require much less memory. Therefore, we might want to prefer using them. 

***

## Exceptions 

An exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions.

### The Catch or Specify Requirement

Valid Java programming language code must honor the Catch or Specify Requirement.

The code that might throw certain exceptions must be enclosed by either of the following:

* A try statement that catches the exception, The try must provide a handler for the exception.
* A method that specifies that it can throw the exception. The method must provide a throws clause that lists the exception.

### The Three Kinds of Exceptions:

1-The checked exception
2-The error exception
3-The runtime exception

## Scanning

We use a Scanner for breaking down formatted input into tokens and translating individual tokens according to their data type.

a scanner uses white space to separate tokens.

