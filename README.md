 #include<stdio.h>

int main(){
   
    long int binaryNumber,decimalNumber=0,j=1,remainder;
    scanf("%ld",&binaryNumber);

    while(binaryNumber!=0){
         remainder=binaryNumber%10;
        decimalNumber=decimalNumber+remainder*j;
        j=j*2;
        binaryNumber=binaryNumber/10;
    }

    printf("%ld",decimalNumber);

    return 0;
}
