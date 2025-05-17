# Ex.No:12(D) JAVA QUEUE
## AIM:
To Write a java program to create vector and read the elements for two vector in java collection.(Use equals method )


## ALGORITHM :
1.	Start the Program
2.	Import `PriorityQueue` and `Scanner`
3.	Define class `Main` with `main` method:
-	a) Initialize `Scanner` to read input
-	b) Create a `PriorityQueue` of integers
4.	Read integer `n` from user input for the number of elements
5.	Use a loop to:
-	a) Read integers and add them to the `PriorityQueue`
6.	Check if the `PriorityQueue` is not empty:
-	a) Remove and display the highest-priority element using `poll()`
7.	Display the remaining elements in the `PriorityQueue`
8.	End.





## PROGRAM:
 ```
Program to implement a JAVA QUEUE using Java
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
            PriorityQueue<Integer> pq = new PriorityQueue<>();
        
	    Scanner sc = new Scanner(System.in);
	    int size = sc.nextInt();
	    for(int i=0; i<size; i++)
	    {
	        pq.add(sc.nextInt());
	    }
	    
	    System.out.println("Display the remove element of PriorityQueue:");
            System.out.println(pq.peek());
            pQueue.remove(pq.peek());
            System.out.println("Display the element of PriorityQueue:\n" + pq);
	}
}

```





## OUTPUT:

![Screenshot 2025-05-17 181822](https://github.com/user-attachments/assets/6952b34f-e0b1-4624-99fe-1ebcbd31d961)


## RESULT:
Thus the java program to create vector and read the elements for two vector in java collection.(Use equals method )was executed successfully.


