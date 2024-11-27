# Sem-4

#include<stdio.h>
#include<math.h>

int check(int);

void main()
{
    int n,prime;
    puts("enter:");
    scanf("%d",&n);
    prime = check(n);

    if(prime == 1)
    {
        printf("prime");
    }
    else
    {
        printf("not prime");
    }
}

int check(int n)
{
    int a;
    for(int i=2;i<=sqrt(n);i++)
    {
        if(n%i==0)
        {
            return 0;
        }

    }
    return 1;
}
