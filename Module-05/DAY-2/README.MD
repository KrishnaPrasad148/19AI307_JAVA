# Ex.No:5(B) TIGHTLY ENCAPSULATED CLASS

## AIM:
To Create a java program to display the value of volume of cylinder get the radius and height value as input and use tightly encapsulated class.

## ALGORITHM :
1.	Start the program.
2.	Define `Cylinder` class:
-	a) Private variables `radius` and `height`
-	b) `setRadius(int r)` and `setHeight(int h)` methods to set values
-	c) `getVolume()` method:
- i) Calculate and print `volume = pi * radius * radius * height`
3.	In `Main` class `main` method:
-	a) Use `Scanner` to read `radius` and `height`
-	b) Create `Cylinder` object, set values, and call `getVolume()`
4.	End







## PROGRAM:
 ```
Program to implement a tightly encapsulated class using Java
Developed by: Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.lang.Math;
import java.util.*;

class Cylinder
{ 
    private int n1; 
    private int n2;
    void setnum1(int num1)
    {
        this.n1=num1;
    }
    void setnum2(int num2)
    {
        this.n2=num2;
    }
    public double getVolume()
    {
        double pi=22.0/7.0;
        double result=pi*n1*n1*n2;  
        return result;
    }
}

public class Main
{
    public static void main(String args[])
    {
        Scanner sc=new Scanner(System.in); 
        int n1=sc.nextInt();
        int n2=sc.nextInt();
        Cylinder c=new Cylinder();
        c.setnum1(n1); 
        c.setnum2(n2); 
        double result = c.getVolume();
        System.out.println("volume of Cylinder is: "+result);
    }
}

```






## OUTPUT:



## RESULT:
Thus a java program to display the value of volume of cylinder get the radius and height value as input and use tightly encapsulated class was executed successfully.



