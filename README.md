# hello-world
I am yash.
#include <stdio.h>

// Function to calculate factorial
unsigned long long factorial(int n) {
    if (n == 0 || n == 1)
        return 1;
    else
        return n * factorial(n - 1);
}

int main() {
    int number;
    unsigned long long fact;

    printf("Enter a non-negative integer: ");
    scanf("%d", &number);

    // Validate input
    if (number < 0) {
        printf("Error: Factorial of negative number doesn't exist.\n");
    } else {
        fact = factorial(number);
        printf("Factorial of %d = %llu\n", number, fact);
    }

    return 0;
}
