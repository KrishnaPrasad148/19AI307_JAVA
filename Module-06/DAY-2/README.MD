# Ex.No:6(B) MULTI-LEVEL INHERITANCE

## AIM:
To Develop a Java program to perform Multilevel Inheritance to calculate the area of circle..

## ALGORITHM :
1.	Start the Program.
2.	Define class `Shapes`:
-	a) Method `print_shape()` to print "Shapes Class"
3.	Define class `Circle` that extends `Shapes`:
-	a) Declare integer `rad`
-	b) Method `get()` to read `rad` from user input
4.	Define class `Area` that extends `Circle`:
-	a) Method `cal()` to calculate `result = 3.14 * rad * rad` and print "Area of Circle is " followed by `result`
5.	In `Main` class `main` method:
-	a) Create `Area` object `obj`
-	b) Call `print_shape()`, `get()`, and `cal()` on `obj` to display shape type, read radius, and calculate area
6.	End


## PROGRAM:
 ```
Program to implement a MultiLevel Inheritance using Java
Developed by: Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java
import java.util.*; 

class Shapes
{
    void print_shape()
    {
        System.out.println("Shapes Class");
    }    
}
      
class Circle extends Shapes
{
    int rad; 
    void get()
    {
        Scanner sc=new Scanner(System.in); 
        rad=sc.nextInt();
    }
}

class Area extends Circle
{ 
    void cal()
    {
        double result=3.14*rad*rad; 
        System.out.println("Area of Circle is "+result);
    }
}

public class Main extends Area
{
    public static void main(String args[])
    {
        Area obj=new Area(); 
        obj.print_shape(); 
        obj.get();
        obj.cal();
    }
}
```






## OUTPUT:

![Screenshot 2025-05-13 180340](https://github.com/user-attachments/assets/f2e61091-3852-4675-b707-8c41045c8724)


## RESULT:
Thus the java program for multi-level inheritance was executed successfully.





