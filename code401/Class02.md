# Arrays, Loops, Imports

## Packages and Import

### Packages

Java classes can be grouped together in packages. A package is the same as the directory.

* Package declaration

   The first statement in a java file must be he package declaration.

* Package declaration syntax

    ```
    package illustration;

    import java.awt.*;

    public class Drawing {
      . . .
    }
    ```

### Imports: three options

* import javax.swing.*;  // Make all classes visible altho only one is used.
* import javax.swing.JOptionPane;  // Make a single class visible.
* 
 ```
   class ImportTest {
    public static void main(String[] args) {
        javax.swing.JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
 }

 ```
 
***

## Different types of loops in Java

* Intro to Loops
  
  In programming languages, looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false.

* For Loop 

  A for loop is a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.

* While Loop 

  The while loop is Java's most fundamental loop statement. It repeats a statement or a block of statements while its controlling Boolean-expression is true.

* Do-While Loop
    
     The do-while loop works just like the while loop except for the fact that the first condition evaluation happens after the first iteration of the loop.







