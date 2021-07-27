# OOP

## Object & Class

### Object

An object is a software bundle of related state and behavior. Software objects are often used to model the real-world objects 

Real-world objects characteristics:

* State  
* Behavior

Software objects are similar to real-world objects.

Software objects characteristics:

* Fields 
* Methods 

### Benefits of software objects:
1. Modularity
2. Information-hiding
3. Code re-use
4. Pluggability and debugging ease

### class

A class is a blueprint or prototype from which objects are created.

```
public class Bicycle {
        
 
    //  fields
    public int cadence;
    public int gear;
    public int speed;
        

    //  constructor
    public Bicycle(int startCadence, int startSpeed, int startGear) {
        gear = startGear;
        cadence = startCadence;
        speed = startSpeed;
    }
        
   
    //  methods
    public void setCadence(int newValue) {
        cadence = newValue;
    }
        
    public void setGear(int newValue) {
        gear = newValue;
    }
        
    public void applyBrake(int decrement) {
        speed -= decrement;
    }
        
    public void speedUp(int increment) {
        speed += increment;
    }
        
}
```
The child class can inherits all the fields and methods from the parent class ex:

```
public class MountainBike extends Bicycle {
        
    // the MountainBike subclass has
    // one field
    public int seatHeight;

    // the MountainBike subclass has
    // one constructor
    public MountainBike(int startHeight, int startCadence,
                        int startSpeed, int startGear) {
        super(startCadence, startSpeed, startGear);
        seatHeight = startHeight;
    }   
        
    // the MountainBike subclass has
    // one method
    public void setHeight(int newValue) {
        seatHeight = newValue;
    }   

}
```

***
## Binary, Decimal and Hexadecimal Numbers

* Binary is Base 2, That represent any number using 2 digits (0–1).
* Decimal is Base 10, That represent any number using 10 digits (0–9).
* Hexadecimal is Base 16, That represent any number using 10 digits and 6 characters (0–9, A, B, C, D, E, F).






