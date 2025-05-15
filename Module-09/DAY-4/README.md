# Ex.No:9(D) TRANSIENT ---SERILIZATION

## AIM:
 To implement a Java program to perform Transient in Employee details in Serializable interface to make its object serialized.

## ALGORITHM :
1.	Get employee name and designation from the user.
2.	Save the Employeeinfo object to emp.txt.
3.	Read the object back from emp.txt.
4.	Print employee name and designation (designation is null due to transient).
5.	Delete File: Delete emp.txt and handle any exceptions while trying to read it.




## PROGRAM:
 ```
Program to implement a Transient using Java
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.io.*; 
import java.util.*;

class Employeeinfo implements Serializable
{
    String name; 
    transient String desig;
    Employeeinfo(String n, String r)
    {
        this.name = n; 
        this.desig = r;
    }
}

public class Main
{
    public static void main(String[] args)
    {
        File file = new File("emp.txt"); 
        
        try
        {
            Scanner sc=new Scanner(System.in); 
            String name=sc.nextLine();
            String dept = sc.nextLine();
            Employeeinfo si1 = new Employeeinfo(name,dept); 
            FileOutputStream fos = new FileOutputStream("emp.txt"); 
            ObjectOutputStream oos = new ObjectOutputStream(fos); 
            oos.writeObject(si1);
            oos.close();
        }
        catch (Exception e)
        {
            System.out.println(e);
        }
        
        Employeeinfo si=null;
        try
        {
            FileInputStream fis = new FileInputStream("emp.txt"); 
            ObjectInputStream ois = new ObjectInputStream(fis); 
            si = (Employeeinfo)ois.readObject();
        }
        catch (Exception e)
        {
            e.printStackTrace();
        }
        
        System.out.println("Transient--Employee Name:"+si.name); 
        System.out. println("Transient--Employee Designation:"+si.desig);
        
        try
        {
            file.delete();
            FileInputStream fi = new FileInputStream("emp.txt"); 
            DataInputStream di = new DataInputStream(fi);
            int b=di.readInt();
        }
        catch (Exception e)
        {
            System.out.println("Exception: " +e); 
        }
    }
}

```






## OUTPUT:



## RESULT:
Thus, implementation of a Java program to perform Transient in Employee details in Serializable interface to make its object serialized was executed and verified successfully.

