# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
1.Start the program and import the required libraries. <br>
2.Seed the random number generator using the current time(i.e) rand(time(0));<br>
3.Get the number of random number and range to generate.<br>
4.Pass the value for number of iterations and print the numbers.<br>
5.End the program.

# PROGRAM:
```
Developed by : Keerthika s
Register Number: 212223040093
```
```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    int n, i, lower, upper;
    srand(time(0));
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &n);
    printf("Enter the lower limit: ");
    scanf("%d", &lower);
    printf("Enter the upper limit: ");
    scanf("%d", &upper);
    printf("Generated random numbers:\n");
    for (i = 0; i < n; i++) {
        int random_num = (rand() % (upper - lower + 1)) + lower;
        printf("%d\n", random_num);
    }
    return 0;
}
```
# OUTPUT:
![image](https://github.com/user-attachments/assets/ced13012-9a78-4339-808b-5a9cd64f66a6)

# RESULT:
Thus the program is created and executed successfully.
