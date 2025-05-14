# Ex.No:7(E)  POLYMORPHISM

## AIM:
To implement method overloading in Java to calculate the sum of two and three numbers demonstrating compile-time polymorphism
## ALGORITHM :
1.	Start the program.
2.	Create a class named SumExample.
3.	Inside the class, define:
     a.	A method sum(int a, int b) to calculate the sum of two numbers.
     b.	An overloaded method sum(int a, int b, int c) to calculate the sum of three numbers.
4.	In the main() method:
      a.	Create an object of the SumExample class.
      b.	Call both versions of the sum() method with appropriate arguments.
      c.	Print the results.
5.	End the program.



## PROGRAM:
 ```
Program to implement a Method Overloading in Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*;

class Calculation
{
    void sum(int a,int b)
    {
        System.out.println(a+b);
    }
    void sum(int a,int b,int c)
    {
        System.out.println(a+b+c);
    }
}


public class Main
{
    public static void main(String []args)
    {
        Calculation obj=new Calculation();
        Scanner sc=new Scanner(System.in);
        int a=sc.nextInt();
        int b=sc.nextInt();
        int c=sc.nextInt();
        obj.sum(a,b);
        obj.sum(a,b,c);
    }
}

```






## OUTPUT:

![Screenshot 2025-05-14 141657](https://github.com/user-attachments/assets/f85b64ca-b8b1-472c-95b7-7d01abd0b331)


## RESULT:

Thus the  java program successfully demonstrates method overloading, showing compile-time polymorphism by calculating the sum of two and three numbers using methods with the same name but different parameter lists..


