# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
If an Integer object is set to null, and you attempt to call .toString() on it, what happens? How can you prevent your code from throwing an exception in such cases?

## AIM:
To write a Java program to demonstrate NullPointerException when calling .toString() on a null Integer object and to handle the exception using try-catch

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read an integer value from the user.
4.	Assign null if the user enters 0 (or a specific case).
5.	Try to call .toString() method on the Integer object.
6.	.Catch the NullPointerException and display a meaningful message.
7.	Display output and end the program.





## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: Divyashree B
RegisterNumber:  212224040081
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class NullCheck
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        Integer num = sc.nextInt(); 
        try 
        {
            if (num == 0) 
            {
                num = null;
            }
            System.out.println(num.toString());

        } 
        catch (NullPointerException e) 
        {
            System.out.println("Null Integer");
        }
    }
}

```






## OUTPUT:




<img width="580" height="341" alt="image" src="https://github.com/user-attachments/assets/06fa15b5-0373-4c52-a6c4-5b6b36a70d48" />








## RESULT:
Therefore the program has been executed successfully.
