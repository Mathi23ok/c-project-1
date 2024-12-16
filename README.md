# c-project







#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main(){
    int guess,random;
    int n=0;
    srand(time(NULL));
    printf("Welcome to the number guessing game ^-^ :");
    random = rand()%100 + 1;//generating number between 0 to 100;
    printf("%d",random);
    do{
    printf("\nGuess a number between 1 to 100 :");
    scanf("%d",&guess);
    n++;
    if(guess>random){
        printf("guess a smaller one \n");
    }else if(guess<random){
        printf("guess a larger one \n");
        
    }else{
        printf("Wow, you have guessed the number in %d attempts \n",n);
    }
    }while(guess!=random);
        printf("Thank u for playing\n");
        printf("Developed by : Sanju");
    
}
