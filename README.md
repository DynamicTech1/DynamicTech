//A c programming language compound interest program by Dynamic Tech.
#include <stdio.h>
#include <conio.h>
#include <math.h>
int main()
{ 
    printf("Hello and welcome to the Dynamic Tech.");
    printf("\nNamaskar doston mera naam 'DGSushant' hai.");
    char name[20];
    printf("\nEnter your name :");
    fgets(name,20,stdin);
    puts(name);
    char hal_chal;
    printf("Kya hal chal hai sabhi ke?");
    printf("\n'g' for good and 'b' for bad :");
    scanf("%c",&hal_chal);
    if(hal_chal == 'g')
    {
        printf("\nHello %syour welcome to the Dynamic Tech.",name);
    }
    else if (hal_chal == 'b')
    {
        printf("\nHello %s.We do happy your mood.Welcome to the Dynamic Tech",name);
    }
    printf("\nLet's Start.");         
    float principal;
    printf("\nEnter the principal :");
    scanf("%f", &principal);
    float rate;
    printf("\nEnter the rate :");
    scanf("%f", &rate);
    float time;
    printf("\nEnter the time :");
    scanf("%f", &time);
    float formula1 = principal * pow((1 + rate / 100), time);
    float C_I = formula1 - principal;
    printf("\nAmount = %f", formula1);
    printf("\nCompound Interest = %f", C_I);
    return 0;
    getch();
     
}
