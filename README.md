#include<stdio.h>
#include<stdlib.h>
#include<time.h>
int main(){
    int number , guess , nguesses=1;
    srand(time(0));
number =rand()%100 +1;
    do{
        printf("guess the no. btw 1 to 100\n");//generates a random no btw 1 to 100
        scanf("%d" ,&guess);
        if(guess>number){
            printf("lower no please\n");

        }
else if(guess<number){
            printf("higher no please\n");



    }
    else{
    printf("u guessed it in %d attempts\n" , nguesses);
    }
    nguesses++;}
    while(guess!=number);
    return 0;
}
