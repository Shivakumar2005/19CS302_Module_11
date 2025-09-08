# EX 53 C program to remove duplicates in an array.
## DATE:08/09/2005
## AIM:
To write a C program to remove duplicates in an array.

## Algorithm
1. Start the program and declare variables.
2. Read the size of the array and the elements from the user.
3. Traverse each element of the array.
4. Compare the current element with the next elements to check for duplicates. 
5. End the program.  

## Program:
/*
C program to remove duplicates in an array
Developed by: 
RegisterNumber:  
*/

#include <stdio.h>

int main() {
    int arr[100], n, i, j, k;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for(i = 0; i < n; i++) {
        for(j = i + 1; j < n; j++) {
            if(arr[i] == arr[j]) {
                // Shift elements to remove duplicate
                for(k = j; k < n - 1; k++) {
                    arr[k] = arr[k + 1];
                }
                n--;  // reduce size
                j--;  // stay at same index after shifting
            }
        }
    }

    printf("Array after removing duplicates:\n");
    for(i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}


## Output:

<img width="1503" height="676" alt="image" src="https://github.com/user-attachments/assets/29031846-bbc4-481b-a3ef-bb09ab4767a6" />


## Result:
Thus the program was executed and the output was verified successfully.
