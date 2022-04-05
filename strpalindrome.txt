#include <stdio.h>
#include<string.h>
int main()
{
    char a[100];
    scanf("%s",a);
    int flag = 1;
    for(int i=0;i<=strlen(a)/2+1;i++)
        if(a[i] != a[strlen(a)-i-1]) {
            flag=0;
            break;
        }
    printf("%d",flag);
    return 0;
}