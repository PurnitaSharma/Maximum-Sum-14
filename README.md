# Maximum-Sum-14
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>
void sum(int a[],int n)
{
    int i,s=0,max=0;
    for(i=0;i<n;i++)
    {
        s=s+a[i];
        if(s>max)
        {
            max=s;
        }
        if(s<0)
        {
            s=0;
        }
    }
    printf("%d",max);
}
int main() {
    int n;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
        scanf("%d",&a[i]);
    sum(a,n);
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
