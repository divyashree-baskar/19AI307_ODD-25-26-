# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program to define an enum named GameLevel with three constants: EASY, MEDIUM, and HARD.

## AIM:
To write a Java program that defines an enum named GameLevel with constants EASY, MEDIUM, and HARD, and allows the user to select a game level.

## ALGORITHM :
Define an enum GameLevel with constants: EASY, MEDIUM, HARD.

Read user input as a string and convert it to uppercase.

Use GameLevel.valueOf() to match the input with an enum constant.

If the value matches, print the selected game level.

If no match is found, catch IllegalArgumentException and show an error message.

Close the scanner in the finally block.





## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: Divyashree B
RegisterNumber:  212224040081
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

enum GameLevel {
    EASY, MEDIUM, HARD;
}

public class Game {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String userInput = scanner.nextLine().toUpperCase();

        try {
            GameLevel level = GameLevel.valueOf(userInput);
            System.out.println("You selected game level: " + level);
        } catch (IllegalArgumentException e) {
            System.out.println("Invalid game level entered.");
        } finally {
            scanner.close();
        }
    }
}
```





## OUTPUT:

<img width="815" height="326" alt="image" src="https://github.com/user-attachments/assets/5a88eca9-df37-4f4a-94b3-5eba8d899c5a" />



## RESULT:
Therefore the program has been executed successfully.
