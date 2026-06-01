# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to implement a Wrapper Class and check whether a given number is prime or not.

## AIM:
To implement a Wrapper Class (`Integer`) in Java and determine whether the given number is a prime number.

## ALGORITHM:
1. Start the program.
2. Import the necessary package `java.util`.
3. Create a `Scanner` object to read input from the user.
4. Read an integer value using the `Integer` wrapper class.
5. Initialize a boolean variable `isPrime` as `true`.
6. Check whether the number is less than or equal to 1. If so, set `isPrime` to `false`.
7. Otherwise, iterate from 2 to the square root of the number.
8. If the number is divisible by any value in the range, set `isPrime` to `false` and terminate the loop.
9. Check the value of `isPrime`.
10. Display whether the number is prime or not.
11. Close the scanner object.
12. Stop the program.

## PROGRAM:
```java
/*
Program to implement a Wrapper Class using Java
Developed by: Vikamuhan Reddy
RegisterNumber: 212223240181
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Integer num = sc.nextInt(); // Wrapper class

        boolean isPrime = true;

        if (num <= 1) {
            isPrime = false;
        } else {
            for (int i = 2; i <= Math.sqrt(num); i++) {
                if (num % i == 0) {
                    isPrime = false;
                    break;
                }
            }
        }

        if (isPrime) {
            System.out.println(num + " is a prime number.");
        } else {
            System.out.println(num + " is not a prime number.");
        }

        sc.close();
    }
}
```

## OUTPUT:
<img width="526" height="173" alt="Screen Shot 2026-06-01 at 14 19 49" src="https://github.com/user-attachments/assets/37af8888-4cc0-4820-a5f4-795e024658af" />


## RESULT:
Thus, the Java program to implement a Wrapper Class and check whether the given number is prime or not was executed successfully and the output was verified.
