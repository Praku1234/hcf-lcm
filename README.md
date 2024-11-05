# hcf-lcm
#include <stdio.h>
int lcm(int num1, int num2);


int main() {
    int num1, num2;
    int hcfResult, lcmResult;
    

    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
       lcmResult = lcm(num1, num2);
        printf("LCM of %d and %d is: %d\n", num1, num2, lcmResult);


    return 0;
}
int hcf(int num1, int num2) {
    while (num1 != num2) {
        if (num1 > num2)
            num1 -= num2;
        else
            num2 -= num1;
    }
    return num1;
}

// Function to calculate the LCM of two numbers
int lcm(int num1, int num2) {
    return (num1 * num2) / hcf(num1, num2);
}


