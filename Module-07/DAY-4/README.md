# Ex.No:7(D) SYNCHRONIZATION
## AIM:
 To Develop a Java Program to perform static synchronization method for the below Scenario Create a Class Display with synchronized void wish method in that perform "Welcome : Message. Note :Assume Sleep as 400 ms i.e Thread.Sleep(400)
 
## ALGORITHM :
1.	1.	Start the Program.
2.	Define class `Display`:
-	a) Create a `Scanner` object `sc` for input
-	b) Define a synchronized method `wish(String str)`:
- i) Print "Welcome :: " followed by `str` (twice)
3.	End



## PROGRAM:
 ```
Program to implement a Packages using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*;

class Display
{
    synchronized static void wish(String name)
    {
        try
        {
            Thread.sleep(400);
        }
        catch(InterruptedException e)
        {
            e.printStackTrace();
        }
        System.out.println("Welcome :: "+ name);
        System.out.println("Welcome :: "+ name);
    }
}

class Mythread extends Thread
{
    protected String name;
    public Mythread(String name)
    {
        this.name = name;
    }
    
    public void run()
    {
        Display.wish(name);
    }
}

```






## OUTPUT:

![Screenshot 2025-05-14 141226](https://github.com/user-attachments/assets/b0042b2d-5af8-4214-bac3-33de01db4566)


## RESULT:
Thus the java program for synchronization was executed successfully.

