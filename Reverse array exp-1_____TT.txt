// Online C compiler to run C program online
#include <stdio.h>

int main() {
    
    int arr1[5]={1,2,3,4,5};
    int arr2[5]={};
    for(int i=4,j=0;(i>=0 && j<5);i--,j++)
    {
        arr2[j]=arr1[i];
    }
    printf("Actual array : \n");
    for(int i=0;i<5;i++)
    {
        printf("%d ",arr1[i]);
    }
    printf("\n");
    printf("Reversed array : \n");
    for(int i=0;i<5;i++)
    {
        printf("%d ",arr2[i]);
    }
    return 0;
}
