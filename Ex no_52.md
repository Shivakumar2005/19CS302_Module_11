## Task

# Write a function int max_of_four(int a, int b, int c, int d) which reads four arguments and returns the greatest of them.

## Note

There is not built in max function in C. Code that will be reused is often put in a separate function, e.g. int max(x, y) that returns the greater of the two values.

## Input Format

#include <stdio.h>

// Function to return maximum of two numbers
int max(int x, int y) {
    return (x > y) ? x : y;
}

// Function to return maximum of four numbers
int max_of_four(int a, int b, int c, int d) {
    return max(max(a, b), max(c, d));
}

int main() {
    int a, b, c, d;
    scanf("%d %d %d %d", &a, &b, &c, &d);
    printf("%d", max_of_four(a, b, c, d));
    return 0;
}


## Output Format

<img width="1854" height="638" alt="image" src="https://github.com/user-attachments/assets/62cbb85c-c470-4e41-9790-7fea3e7a8cce" />
