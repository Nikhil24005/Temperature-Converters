# Temperature-Converters

#include<stdio.h>
int main(){ 
    float fh, cl;
    int ch;

    printf("\n 1. Convert Temperature Fahrenheit to Celsius.");
    printf("\n 2. Convert Temperature Celsius to Fahrenheit.");
    printf("\n\n Enter Your Choice : ");
    scanf("%d",&ch);

    if(ch==1){
        printf("\n Enter Temperature in Fahrenheit : ");
        scanf("%f",&fh);
        cl = (fh-32)/1.8;
        printf("\n Temperature in Celsius : %f \n ",cl);
    }
    else if(ch==2){
        printf("\n Enter Temperature in Celsius : ");
        scanf("%f",&cl);
        fh = (cl*1.8)+32;
        printf("\n Temperature in Fahrenheit : %f \n",fh); 
    }
    else{
        printf("\n Invalid choice....");
    }
    return 0;
}
