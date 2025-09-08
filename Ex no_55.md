# EX 55 C program to find a square of number using function with arguments without return type.
## DATE:
## AIM:
To write a C program to find a square of number using function with arguments without return type.

## Algorithm
1. Start the program.
2. Define a function that takes an integer argument and prints its square (without return type).
3. In the main function, read a number from the user.
4. Call the function by passing the number as an argument. 
5. Display the square of the given number.  

## Program:
#include <stdio.h>

// Function definition (with arguments, without return type)
void square(int n) {
    printf("Square of %d is: %d\n", n, n * n);
}

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);

    // Function call
    square(num);

    return 0;
}

## Output:

<img width="1346" height="622" alt="image" src="https://github.com/user-attachments/assets/c1a7f82c-2f9e-4e46-9c0d-f7e67fb9c6b8" />


## Result:
Thus the program was executed and the output was verified successfully.
