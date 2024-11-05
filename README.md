# hcf-lcm
#include <stdio.h>
int hcf(int num1, int num2);

int main() {
    int num1, num2;
    int hcfResult, lcmResult;

    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    hcfResult = hcf(num1, num2);
     printf("HCF of %d and %d is: %d\n", num1, num2, hcfResult);

    return 0;
}


