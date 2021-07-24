# Java Basics

## Variables

kinds of variables:

* Instance Variables: Declared without the static keyword.  their values are unique to each object of a class.
* Class Variables: declared with the static keyword, this tells the compiler that there is exactly one copy of this variable in existence.
* Local Variables: store temporary state inside a method.
* Parameters : parameters are always classified as "variables" not "fields". We put parameters inside the parentheses of the method.


## Operators
| Operators	 | Precedence |
| ------ | ----------- |
| postfix | expr++ expr--|
| unary | ++expr --expr +expr -expr ~ !|
| multiplicative | * / %|
| additive | + -|
| shift | << >> >>>|
| relational | < > <= >= instanceof|
| equality | == !=|
| bitwise AND | &|
| bitwise exclusive OR |^|
| bitwise inclusive OR |&#124;|
| logical AND |	&&|
| logical OR|&#124; &#124;|
| ternary|? :|
| assignment|= += -= *= /= %= &= ^= &#124;= <<= >>= >>>=|

## Expressions, Statements, and Blocks

* Expressions: a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value.
* Statements: A statement forms a complete unit of execution.
* Blocks:a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed.

## Control Flow Statements:

The statements inside your source files are generally executed from top to bottom, in the order that they appear. Control flow statements, however, break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code. This section describes the decision-making statements (if-then, if-then-else, switch), the looping statements (for, while, do-while), and the branching statements (break, continue, return) supported by the Java programming language.

## Compiling

Computers use machine language it is represented by a series of 1's and 0's.humans made high level languages because machine language is hard to learn, To make the Computers understand what we write we use compiler to convert our code from high level languages to machine language .
