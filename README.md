#include <stdio.h>
#include <math.h>
int main(){
    double a,b;
    char op,c;
    printf("Enter the Operands: ");
    scanf("%lf %lf",&a,&b);
    printf("Enter the Operator: "); 
    scanf(" %c",&op);
    switch(op) {
    case '+':
        printf("Addition: %.2lf\n",a+b);
        break;
    case '-':
        printf("Subtraction: %.2lf\n",a-b);
        break;
    case '/':
        printf("Division: %.2f\n",(float)a/b);
        break;
    case '*':
        printf("Multiplication: %.2lf\n",a*b);
        break;
    case '%': 
        printf("Remainder: %d",(int)a%(int)b);
        break;
    case '^':
        printf("Power: %lf\n",pow(a,b));
        break;
    default: printf("Wrong operator taken\n");
    }
    return 0;
}
