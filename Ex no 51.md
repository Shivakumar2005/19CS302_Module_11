# EX 51 C program to reverse a string.
## DATE:08/09/2025
## AIM:
To write a C program to reverse a string.

## Algorithm
1. Start the program.
2. Read the input string from the user.
3. Initialize two pointers or indices: one at the beginning and the other at the end of the string.
4. Swap the characters at these positions and move the pointers towards each other until they meet. 
5. Print the reversed string.  

## Program:


#include <stdio.h>
#include <string.h>

int main() {
    char str[100], temp;
    int i, j;

    printf("Enter a string: ");
    scanf("%s", str);

    i = 0;
    j = strlen(str) - 1;

    while (i < j) {
        // Swap characters
        temp = str[i];
        str[i] = str[j];
        str[j] = temp;
        i++;
        j--;
    }

    printf("Reversed string: %s\n", str);

    return 0;
}


## Output:

<img width="1833" height="690" alt="image" src="https://github.com/user-attachments/assets/2f4f6550-85a6-41cf-961b-34e3fab651a9" />


## Result:
Thus the program was executed and the output was verified successfully.
