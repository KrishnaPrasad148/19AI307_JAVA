# Ex.No:7(A)           EXCEPTION HANDLING-RUN TIME EXCEPTION
## AIM:
  To Develop a Java Program for handling Arithmetic Exception (division by zero exception) using Exception Handling Mechanism.

## ALGORITHM :
1.  Start the Program
2.	Import `java.util.*` for input handling
3.	Define class `Example1`:
-	a) In `main` method, create `Scanner` object `sc` for input
4.	Use `try` block to:
-	a) Read integers `a` and `b` from user input
-	b) Calculate `res = a / b` and print "Result: " followed by `res`
5.	Use `catch` block to handle `ArithmeticException`:
-	a) If division by zero occurs, print "You Shouldn't divide a number by zero"
6.	End







## PROGRAM:
 ```
Program to implement a Exception Handling-Run Time Exception using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java
import java.util.*;

public class Main
{
    public static void main(String args[])
    {
        Scanner sc=new Scanner(System.in);
        try
        {
            int a=sc.nextInt(); 
            int b=sc.nextInt(); 
            int res=a/b;

            System.out.println("Result: "+res);
        }
        catch(ArithmeticException e)
        {
            System.out.println("You Shouldn't divide a number by zero");}
        }
}

```






## OUTPUT:

![Screenshot 2025-05-14 140107](https://github.com/user-attachments/assets/defe9c40-c958-4ac3-9334-406db9197716)


## RESULT:
Thus the Java Program for handling Arithmetic Exception (division by zero exception) using Exception Handling Mechanism was executed successfully.

