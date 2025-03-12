# C-4
pascals pattern
#include <stdio.h>
int main()
{
    int n,j,i,s,c;
    printf("enter the rows :");
    scanf("%d", &n);
    for (i=0;i<n;i++){
        for(s=1;s<=n-i;s++){
           printf(" ");
           c=1;
        }
        for(j=0;j<=i;j++){ 
           printf("%d ", c);
           c=c*(i-j)/(j+1);
        }
        printf("\n");
    }
    return 0;
}
