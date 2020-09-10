#include <stdio.h>
#include <cs50.h>

int main(void){
    int height, row;
    
    do {
    height = get_int("please state a height value: ");
    }
    while (height < 1 || height > 8);
    
    for ( row = 0; row < height; row++ ) {
        for ( int space = height - 1; row < space ; space--) {
            printf (" ");
        }
        for ( int hash = -1; hash < row; hash++ ){
            printf ("#");
        }
        for ( int space2 = 0; space2 < 1; space2++ ) {
            printf("  ");
        }
        for ( int hash2 = -1; hash2 < row; hash2++){
            printf("#");
        }
    printf("\n");  
    }
}   
