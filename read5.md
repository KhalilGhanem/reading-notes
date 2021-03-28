# Operators and Loops

## comparison operator:

### evaluating conditions :

we can evaluate a situation by comparing one value in the script to what expect it might be.

*The result will be boolean.*

```
Operators compares two values:
Is Equal to == "see if the values are the same"
Strict Equal to === "check the both data type and the value are the same"
Is not Equal to != "see if the values are not the same"
Strict not Equal === "check the both data type and the value are not the same"
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
## Loops:

Loops check a condition. if it returns true a code block will rund. then will check it again and repeats until the condition returns false 

### For loop structure:
 for(var i=0; i <=5 ;i++){
     console.log(i);
 }
* intialization: var i =0;
* condition: i <=5;
* update: i++;

