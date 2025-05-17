# Ex.No:12(E)  JAVA DEQUEUE

## AIM:
To demonstrate how to remove and display the first element from a Deque using the pollFirst() method in Java Collections with String values.
## ALGORITHM :

1.	Import java.util.*.
2.	Create a Deque using LinkedList.
3.	Add several string elements to the deque.
4.	Use pollFirst() to remove and return the first element.
5.	Print the removed element.
6.	Display the remaining elements in the deque.

## PROGRAM:
 ```
Program to implement a JAVA DEQUEUE
Developed by:  Krishna Prasad S
RegisterNumber:  212223230108
```

## Sourcecode.java:

```java

import java.util.*;

public class deQueueDemo
{
	public static void main(String args[])
	{
            Deque<String> dq = new ArrayDeque<String>();
        
	    Scanner sc=new Scanner(System.in);
	    int size=sc.nextInt();
	    sc.nextLine();
	    for(int i=0;i<size;i++)
	    {
	        dq.offer(sc.next());
	    }
	    System.out.println("Display the element of Dequeue:");
            System.out.println(dq);
            System.out.println(dq.getFirst());
	}
}

```





## OUTPUT:

![Screenshot 2025-05-17 182106](https://github.com/user-attachments/assets/8ce2cbe3-5c35-4d84-b714-fae2452630b5)


## RESULT:

Thus the java program successfully demonstrates how to use pollFirst() to remove and display the first element from a Deque of strings.


