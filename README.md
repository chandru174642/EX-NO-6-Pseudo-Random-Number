# EX-NO-6-Pseudo-Random-Number
## NAME: CHANDRU.P
## REG NO: 212223110007
# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    int count, min, max;

    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);

    printf("Enter the minimum value: ");
    scanf("%d", &min);

    printf("Enter the maximum value: ");
    scanf("%d", &max);

    srand(time(NULL));

    printf("Pseudorandom numbers:\n");
    for (int i = 0; i < count; i++) {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }

    return 0;
}
```

# OUTPUT:
![Screenshot 2025-04-15 141532](https://github.com/user-attachments/assets/a7b1bdb2-01b0-4712-8620-bbf9fdd3c5f7)


# RESULT:
Thus the above given program executed sucessfully.
