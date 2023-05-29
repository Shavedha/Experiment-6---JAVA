# Experiment-6---JAVA
## AIM
To Write a Java program to calculate the power of a number raised to other using recursion where the numbers a and b are to be entered by the user.

## ALGORITHM
1. Create a Java class and declare a static method to calculate the power. Let's name the class PowerCalculator.
2. Inside the PowerCalculator class, define the recursive method calculatePower that takes two parameters: the base number a and the exponent b. 
3. This method will return the result of a raised to the power of b.
4. In the calculatePower method, define the base case: if the exponent b is equal to 0, return 1 since any number raised to the power of 0 is 1.
5. In the recursive case, recursively call the calculatePower method with the base number a and the exponent b-1. Multiply the result of the recursive call with the base number a and return the result.
6. In the main method of the PowerCalculator class, prompt the user to enter the base number a and the exponent b using Scanner class.
7. Call the calculatePower method with the entered values of a and b, and store the result in a variable. Finally, print the result.

## PROGRAM
```
import java.util.Scanner;

public class powerCalculator {
    public static int calculatePower(int a, int b) {
        // Base case
        if (b == 0) {
            return 1;
        }

        // Recursive case
        return a * calculatePower(a, b - 1);
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the base number: ");
        int a = scanner.nextInt();

        System.out.print("Enter the exponent: ");
        int b = scanner.nextInt();

        int result = calculatePower(a, b);
        System.out.println(a + " raised to the power of " + b + " is: " + result);

        scanner.close();
    }
}
```
## OUTPUT
<img width="374" alt="image" src="https://github.com/Shavedha/Experiment-6---JAVA/assets/93427376/a299ae81-eab6-4272-b127-5b90794a4b81">

## RESULT
Thus power of a number is calculated using Java programming language.
