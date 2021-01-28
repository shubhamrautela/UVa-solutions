#include<stdio.h>

int maximum(int x);

int main(){
    int i,j,curr,max,x,y;
    curr = max = 0;
    while((scanf("%d %d", &i, &j)) >= 0){
        curr = max = 0;
        x = (i<j)?i:j;
        y = (i<j)?j:i;
        for(;x <= y ; x++){
           curr = maximum(x);
           if(curr > max){
                max = curr;
           }
        }
        printf("%d %d %d\n", i, j, max);
    }
    return 0;
}

int maximum(int x){
    int count = 1;
    while(x != 1){
        count++;
        if(x % 2==0){
            x/=2;
        }
        else x = 3*x + 1;
    }
    return count;
}
