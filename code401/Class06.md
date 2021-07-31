# Inheritance and Interfaces

## Inheritance
Different kinds of objects often have a certain amount in common with each other.

Object-oriented programming allows classes to inherit commonly used state and behavior from other classes.


```
ex: Bicycle is the superclass of MountainBike, RoadBike, and TandemBike

                 Bicycle 
                    |
      ----------------------------
      |             |            |
MountainBike    RoadBike     TandemBike

```

**Each class is allowed to have one direct superclass, and each superclass has the potential for an unlimited number of subclasses**

```
-The syntax for creating a subclass

class MountainBike extends Bicycle {

    // new fields and methods defining 
    // a mountain bike would go here

}
```
## Interface
an interface is a group of related methods with empty bodies.

```
ex:

interface Bicycle {

    //  wheel revolutions per minute
    void changeCadence(int newValue);

    void changeGear(int newValue);

    void speedUp(int increment);

    void applyBrakes(int decrement);
}
```
To implement this interface we need a new class with implements keyword in the class declaration.
```
class ACMEBicycle implements Bicycle {

    int cadence = 0;
    int speed = 0;
    int gear = 1;

   // The compiler will now require that methods
   // changeCadence, changeGear, speedUp, and applyBrakes
   // all be implemented. Compilation will fail if those
   // methods are missing from this class.

    void changeCadence(int newValue) {
         cadence = newValue;
    }

    void changeGear(int newValue) {
         gear = newValue;
    }

    void speedUp(int increment) {
         speed = speed + increment;   
    }

    void applyBrakes(int decrement) {
         speed = speed - decrement;
    }

    void printStates() {
         System.out.println("cadence:" +
             cadence + " speed:" + 
             speed + " gear:" + gear);
    }
    ````