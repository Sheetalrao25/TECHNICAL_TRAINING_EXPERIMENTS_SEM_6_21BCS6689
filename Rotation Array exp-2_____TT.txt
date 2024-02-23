#include <stdio.h>
int main() {
    
    int arr1[5]={1,2,3,4,5};
    int arr2[5]={};
    int d;
    int temp;
    printf("Enter how many rotations you want : ");
    scanf("%d",&d);
    printf("Array Before Rotation : \n");
    for(int i=0;i<5;i++)
    {
        printf("%d ",arr1[i]);
    }
    

    for(int i=0;i<d;i++)
    {
        temp=arr1[0];
        for(int j=0,k=1;(j<4 && k<5);j++,k++)
        {
            arr1[j]=arr1[k];
        }
        arr1[4]=temp;
    }
    printf("\n");
    printf("After Rotation the array : \n");
    for(int i=0;i<5;i++)
    {
        printf("%d ",arr1[i]);
    }
    return 0;
}
