**
# 19AI308-Object-Oriented-Programming-using-CSharp--Ex7---Hierarchical-Inheritance

# AIM:

To write a C# program to implement heirarchical inheritance for the following problem statement:  All the vehicles need Tyres on their wheels. 
So, the manufacturer designs their vehicle as they want and import Tyre from its base class and fit it into Wheels. 
They don’t need to design Tyre all the time. Once they designed the model and use it various times. 
Aim is to create a Scooter and Car vehicle where the Tyre is being inherited from vehicle class.

## ALGORITHM :

### Step 1 :

Define a base class 'Vehicle' with a method 'tyre' to describe tyres.

### Step 2 :

Create a 'Scooter' class inheriting 'Vehicle', with a method 'Display' and 'tyres'.

### Step 3 :

Implement 'Display' to show class type and call base 'tyre'.

### Step 4 :

Similarly, make a 'Car' class inheriting 'Vehicle', with a 'Display' method.

### Step 5 :

Instantiate Car' and 'Scooter', call 'Display' with respective tyre counts.



# PROGRAM:

## DEVELOPED BY : DODDA JAYASRI
## REG NO: 212222240028
```
using System;

public class Vechicle
{
    public void tyre()
    {
        Console.WriteLine("It is a tubeless tyre");
    }
}

class Scooter : Vechicle
{
    public  void display() 
    {
        base.tyre();
        Console.WriteLine("It is a scooter class");
    }
}

class Car : Vechicle
{
    public  void display() 
    {
        base.tyre();
        Console.WriteLine("It is a car class");
    }
}

class Program
{
    static void Main()
    {
        Scooter scooter = new Scooter();
        Car car = new Car();
        
        
        Console.WriteLine("Scooter started:");
        scooter.display();
        
        Console.WriteLine("\nCar started:");
        car.display();
    }
}
```

# OUTPUT:

![Screenshot 2024-04-22 221058](https://github.com/22008686/19AI308-Object-Oriented-Programming-using-CSharp--Ex7---Hierarchical-Inheritance/assets/118916413/32f6457b-12a9-4871-9b33-1f9659868a6c)

# RESULT:

Thus the program has been executed successfully.
**
