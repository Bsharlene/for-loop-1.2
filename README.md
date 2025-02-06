#include <stdio.h>

int main ()
{
    int n, i, j;
    printf("How many rows you want to your pyramid?\n");
    scanf("%d", &n);
    
    for(i = 1; i <=  n; i++)
    {
        for(j = 1; j <= 2*n-1; j++)
        {
             if (j >= n-(i - 1) && j <= n+(i - 1))
            {
            printf("*");
            }
            else
                printf(" ");
        }
        printf("\n");
    }
    return 0;
}



import java.util.Scanner;

public class SimpleCalculator {
    public static void main(String[] args) {
        // Create a Scanner object to read input
        Scanner scanner = new Scanner(System.in);

        // Prompt the user to enter the first number
        System.out.print("Enter the first number: ");
        double input1 = scanner.nextDouble();

        // Prompt the user to enter the second number
        System.out.print("Enter the second number: ");
        double input2 = scanner.nextDouble();

        // Calculate the sum, difference, product, and quotient
        double sum = input1 + input2;
        double difference = input1 - input2;
        double product = input1 * input2;
        double quotient = 0;

        // Check for division by zero
        if (input2 != 0) {
            quotient = input1 / input2;
        } else {
            System.out.println("Cannot divide by zero.");
        }

        // Output the results
        System.out.println("Sum: " + sum);
        System.out.println("Difference: " + difference);
        System.out.println("Product: " + product);
        if (input2 != 0) {
            System.out.println("Quotient: " + quotient);
        }

        // Close the scanner
        scanner.close();
    }
}


