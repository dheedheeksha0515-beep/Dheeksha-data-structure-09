# Dheeksha-data-structure-09
#include <stdio.h>

int main(){
    int book[5]={45,20,60,10,30};
    int i,j,key;

    for(i=1;i<5;i++){
        key=book[i];
        j=i-1;

        while(j>=0 && book[j]>key){
            book[j+1]=book[j];
            j--;
        }

        book[j+1]=key;
    }

    printf("Sorted Book IDs:\n");
    for(i=0;i<5;i++)
        printf("%d ",book[i]);

    return 0;
}
Sorted Book IDs:
10 20 30 45 60
