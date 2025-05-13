# Ex.No:6(E)  MULTIPLE INHERITANCE

## AIM:
To write a Java program using multiple inheritance through interfaces to read student details and marks, calculate the average, and display the mark sheet.

## ALGORITHM :

1.	Start the program.
2.	Create interface Student:
a.	Declare methods to read name and rollno.
3.	Create interface Studentdet:
a.	Declare a method to read marks of 6 subjects and calculate the average.
b.	Create a class Studentdetails that implements both interfaces:
c.	Define variables for name, roll number, marks array, and average.
4.	Implement all methods from the interfaces.
a.	Create a display() method to show student details and average.
5.	In main() method:
a.	Create an object of Studentdetails.
b.	Call the methods to get input and display results.
6.	End the program.


## PROGRAM:
 ```
Program to implement a Multiple Inheritance
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:
```java

import java.util.*;

interface Student
{
    public abstract void getdetails1();
}
interface Studentdet
{
    public abstract void getdetails2();
}

class Studentdetails implements Student,Studentdet
{
    Scanner sc=new Scanner(System.in);
    int rollno;
    String name;
    int marks[]=new int[6];
    int avg,sum=0;
   
    public void getdetails1()
    { 
        rollno=sc.nextInt();
        name=sc.next();
        System.out.println("Roll No : " +rollno);
        System.out.println("Name : " +name);
    }
    public void getdetails2()
    {   
        for(int i=0;i<6;i++)
        {
            marks[i]=sc.nextInt();
            sum=sum+marks[i];
        }
        avg=sum/6;
        System.out.println("Average  : " +avg);
    }
    public void display()
    {
        getdetails1();
        getdetails2();
    }
}
public class Main
{
	public static void main(String[] args) 
	{
	    Studentdetails obj = new Studentdetails(); 
            obj.display(); 
	}
}

```






## OUTPUT:

![Screenshot 2025-05-13 181359](https://github.com/user-attachments/assets/86eabf15-b2d5-4ae9-9f7a-50c7b41de3f1)


## RESULT:

Thus, the java program demonstrates multiple inheritance using interfaces and successfully displays the mark sheet of a student by collecting personal and academic data. 
