# Ex.No:5(A)  DATA HIDING AND ENCAPSULATION
## AIM:
To Create a java program to display name and location of the employee and use the encapsulation concepts

## ALGORITHM :
1.  Start the program
2.	Define class `Employee`:
-	a) Declare two private `String` variables: `name1` and `name2`
-	b) Define `setname(String n1)` method to set `name1` to `n1`
-	c) Define `setname2(String n2)` method to set `name2` to `n2`
-	d) Define `get1()` method to return `name1`
-	e) Define `get2()` method to return `name2`
3.	Define `Main` class with `main` method:
-	a) Create `Scanner` object `sc` for input
-	b) Read `name1` and `name2` from user input
-	c) Create ` Employee ` object `hl`
-	d) Use `hl.setname(name1)` and `hl.setname2(name2)` to set the names
-	e) Print the values of `hl.get1()` and `hl.get2()`
4.	End





## PROGRAM:
 ```
Program to implement a Data Hiding & Encapsulation using Java
Developed by: Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*;

class hidden_love
{
    private String name1; 
    private String name2;
    void setname(String n1)
    {
        name1=n1;
    }
    void setname2(String n2)
    {
        name2=n2;
    }
    public String get1()
    {
        return name1;
    }
    public String get2()
    {
        return name2;
    }
}

public class Main
{
    public static void main(String args[])
    {
        Scanner sc=new Scanner(System.in); 
        String name1=sc.nextLine();
        String name2=sc.nextLine(); 
        hidden_love hl=new hidden_love();
        hl.setname(name1);
        hl.setname2(name2); 
        System.out.println(hl.get1()); 
        System.out.println(hl.get2());
    }
}

```






## OUTPUT:
![Screenshot 2025-05-13 165657](https://github.com/user-attachments/assets/82a659da-c767-4c9a-80e6-f3ada7ade1f7)



## RESULT:
Thus , the  java program to display name and location of the employee and use the encapsulation concepts executed successfully.
