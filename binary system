#include <stdio.h>
int binary(int bn1, int bn2)
{
    int i = 0, rem = 0, a[20];
    int prod = 0;
 
    while (bn1 != 0 || bn2 != 0)
    {
        a[i++] =(bn1 % 10 + bn2 % 10 + rem) % 2;
        rem =(bn1 % 10 + bn2 % 10 + rem) / 2;
        bn1 = bn1 / 10;
        bn2 = bn2 / 10;
    }
    if (rem != 0)
        a[i++] = rem;
    --i;
    while (i >= 0)
        prod = prod * 10 + a[i--];
    return prod;
}
 
int main()
{
 
    long bn1, bn2,multiply=0;
   
    int i = 0, rem = 0, a[20], digit, factor = 1;
    while(1){
    printf("Enter the Choice :\n");
    printf("1.Addition\n2.Multiplication\n3.Exit\n");
    int n;
      scanf("%d",&n);
      if(n==1){
           printf("Enter the first binary number: ");
    scanf("%ld", &bn1);
    printf("Enter the second binary number: ");
    scanf("%ld", &bn2);
    while (bn1 != 0 || bn2 != 0)
    {
        a[i++] =(bn1 % 10 + bn2 % 10 + rem) % 2;
        rem =(bn1 % 10 + bn2 % 10 + rem) / 2;
        bn1 = bn1 / 10;
        bn2 = bn2 / 10;
    }
    if (rem != 0)
        a[i++] = rem;
    --i;
    printf("Sum of two binary numbers: ");
    while (i >= 0)
        printf("%d", a[i--]);

      printf("\n");}

      else if(n==2){
              printf("Enter the first binary number: ");
    scanf("%ld", &bn1);
    printf("Enter the second binary number: ");
    scanf("%ld", &bn2);
    while (bn2 != 0)
    {
        digit =  bn2 % 10;
        if (digit == 1)
        {
            bn1 = bn1 * factor;
            multiply = binary(bn1, multiply);
        }
        else
            bn1 = bn1 * factor;
        bn2 = bn2 / 10;
        factor = 10;
    }
    printf("Product of two binary numbers: %ld", multiply);
    printf("\n");

      }
      else if(n==3){
          break;
      }
    }
    return 0;
}
